---
title: Probleem met PRT oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330954"
---
# <a name="troubleshoot-prt-issue"></a>Probleem met PRT oplossen

Voor elk apparaat dat wordt geverifieerd, moet het volledig zijn geregistreerd en in goede staat zijn en een prt (Primary Refresh Token) kunnen verkrijgen.

Voor het registratieproces voor hybride Azure AD-joins moeten apparaten zich op een bedrijfsnetwerk hebben. Het werkt ook via VPN, maar daar zijn enkele kanttekeningen bij. We hebben gehoord dat klanten hulp nodig hebben bij het oplossen van problemen met het hybride Azure AD-registratieproces onder externe werkomstandigheden. Hier volgen een overzicht van wat er 'onder de motorkap' gebeurt tijdens het registratieproces.

**Cloudverificatieomgeving (met behulp van Wachtwoordhashsynchronisatie van Azure AD of pass-through-verificatie)**

Deze registratiestroom wordt ook wel 'Synchronisatie deelnemen' genoemd.

1. Windows 10 wordt een SCP-record ontdekt wanneer gebruikers zich aanmelden bij het apparaat.
    1. Het apparaat probeert eerst tenantgegevens op te halen uit SCP aan clientzijde in register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Als dit mislukt, communiceert het apparaat met on-premises Active Directory (AD) om tenantgegevens op te halen bij Service Connection Point (SCP). Als u SCP wilt controleren, raadpleegt u dit [document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Opmerking:** Het is raadzaam SCP in te stellen in de AD en alleen SCP aan de clientzijde te gebruiken voor de eerste validatie.

2. Windows 10 probeert te communiceren met Azure AD onder de systeemcontext om zichzelf te verifiëren tegen Azure AD. U kunt controleren of het apparaat toegang heeft tot Microsoft-resources onder het systeemaccount met behulp van het script Test Device Registration Connectivity.

3. Windows 10 genereert een zelf ondertekend certificaat en slaat het op onder het computerobject in on-premises AD. Hiervoor is een gezichtslijn vereist voor domeincontroller.

4. Een apparaatobject met een certificaat wordt gesynchroniseerd met Azure AD via Azure AD Verbinding maken. Synchronisatiecyclus is standaard elke 30 minuten, maar is afhankelijk van de configuratie van Azure AD-Verbinding maken. Raadpleeg dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In dit stadium kunt u het onderwerpapparaat in de status 'In behandeling' zien onder Apparaatblad van Azure Portal.

6. Bij de volgende gebruiker die zich aanmeld bij Windows 10, wordt de registratie voltooid. 

**Opmerking:** Als u VPN gebruikt en een aanmeldingsproces voor aanmelding de domeinconnectiviteit beëindigt, kunt u registratie handmatig activeren:
 1. Een dsregcmd /join lokaal op admin prompt of op afstand via PSExec naar uw pc. Bijvoorbeeld: PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Zie Problemen met apparaten oplossen voor meer informatie over problemen met hybride [joins.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
