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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573493"
---
# <a name="troubleshoot-prt-issue"></a>Probleem met PRT oplossen

Om te voorkomen dat een apparaat wordt geverifieerd, moet het volledig geregistreerd en in goede staat zijn en kan een primaire vernieuwings token (PRT) worden verkregen.

Voor het Hybrid Azure AD-registratieproces zijn apparaten in een bedrijfsnetwerk vereist. Dit werkt ook via VPN, maar er is een aantal voorbehoud. We willen klanten weten dat ze hulp nodig hebben bij het oplossen van problemen bij het registreren van het hybride Azure AD join-registratieproces onder externe werkomstandigheden. Dit is een uitsplitsing van wat er gebeurt onder de oppervlakte tijdens het registratieproces.

**Cloud verificatie omgeving (via Azure AD Password Hash sync of Pass Through-verificatie)**

Deze registratie stroom wordt ook wel ' synchronisatie deelnemen ' genoemd.

1. Windows 10 detecteert een SCP-record bij gebruikers die zich bij het apparaat aanmelden.
    1. Het apparaat probeert eerst Tenant informatie op te halen uit de clientzijde-SCP in het register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Zie dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)voor meer informatie.
    2. Als dit mislukt, communiceert het apparaat met on-premises Active Directory (AD) om Tenant informatie op te halen van het service verbindingspunt (SCP). Als u SCP wilt controleren, raadpleegt u dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> U wordt aangeraden SCP in te schakelen in de advertentie en uitsluitend aan clientzijde-SCP te gebruiken voor initiële verificatie.

2. Windows 10 probeert met Azure AD te communiceren onder de systeemcontext om zichzelf te verifiëren tegen Azure AD. U kunt controleren of het apparaat toegang heeft tot Microsoft-bronnen onder het systeemaccount met behulp van het script voor het registreren van apparaten.

3. In Windows 10 wordt een zelfondertekend certificaat gegenereerd en opgeslagen onder het computerobject in on-premises advertenties. Dit vereist regel-van-gezichtsvermogen voor domein controller.

4. Een apparaatobject met een certificaat wordt gesynchroniseerd met Azure AD via Azure AD Connect. De synchronisatie cyclus is standaard elke 30 minuten, maar dit is afhankelijk van de configuratie van Azure AD Connect. Raadpleeg dit [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)voor meer informatie.

5. In dit stadium ziet u mogelijk het onderwerp-apparaat in de status in behandeling onder apparaatprofielen van Azure Portal.

6. Bij de volgende gebruikersaanmelding met Windows 10 wordt de registratie beëindigd. 

> [!NOTE]
> Als u een VPN-verbinding hebt en een proces voor afmelden afmelden de domein verbinding beëindigt, kunt u de registratie handmatig activeren:
 1. Meld u op een dsregcmd-/join lokale vragen of extern via PSExec op uw PC. Bijvoorbeeld PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. Zie [problemen met apparaten oplossen](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)voor meer informatie over problemen met hybride verbindingen.
