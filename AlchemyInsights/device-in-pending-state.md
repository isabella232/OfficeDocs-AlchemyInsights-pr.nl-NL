---
title: Apparaat in status in behandeling
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330367"
---
# <a name="device-in-pending-state"></a>Apparaat in status in behandeling

**Vereisten:**

1. Als u apparaatregistraties voor de eerste keer instelt, controleert u of u Inleiding tot apparaatbeheer hebt bekeken [in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) die u begeleidt bij het krijgen van apparaten onder beheer van Azure AD.
2. Als u apparaten rechtstreeks registreert bij Azure AD en deze registreert bij Intune, moet u ervoor zorgen [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) dat u [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) hebt geconfigureerd en eerst de licenties hebt.
3. Controleer of u gemachtigd bent om bewerkingen uit te voeren in Azure AD en on-premises AD. Alleen een globale beheerder in Azure AD kan instellingen voor apparaatregistraties beheren. Als je automatische registraties in je on-premises Active Directory instelt, moet je bovendien een beheerder zijn van Active Directory en AD FS (indien van toepassing).

Voor het hybride registratieproces voor Azure AD-joins moeten apparaten zich op het bedrijfsnetwerk hebben. Het werkt ook via VPN, maar er zijn enkele kanttekeningen. We hebben gehoord dat klanten hulp nodig hebben bij het oplossen van problemen met het hybride Azure AD-registratieproces onder externe werkomstandigheden.

**Cloudverificatieomgeving (met behulp van Wachtwoordhashsynchronisatie van Azure AD of pass-through-verificatie)**

Deze registratiestroom wordt ook wel 'Synchronisatie deelnemen' genoemd.

Hier vindt u een overzicht van wat er gebeurt tijdens het registratieproces:

1. Windows 10 wordt de SCP-record (Service Connection Point) ontdekt wanneer de gebruiker zich aanmeldt bij het apparaat.

    1. Het apparaat probeert eerst tenantgegevens op te halen uit SCP aan clientzijde in register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Zie document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Als dit mislukt, communiceert het apparaat met on-premises Active Directory om tenantgegevens van SCP op te halen. Als u SCP wilt controleren, raadpleegt u dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Opmerking:** Het is raadzaam SCP in te stellen in de Active Directory en alleen SCP aan de clientzijde te gebruiken voor eerste validatie.

2. Windows 10 probeert te communiceren met Azure AD onder de systeemcontext om zich te verifiëren tegen Azure AD.

    U kunt controleren of het apparaat toegang heeft tot Microsoft-resources onder het systeemaccount met behulp van het [script Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genereert zelf ondertekend certificaat en slaat het op onder het computerobject in on-premises Active Directory. Hiervoor is een gezichtslijn vereist voor domeincontroller.

4. Apparaatobject met certificaat wordt gesynchroniseerd met Azure AD via Azure AD Verbinding maken. Synchronisatiecyclus is standaard elke 30 minuten, maar is afhankelijk van de configuratie van Azure AD-Verbinding maken. Raadpleeg dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In dit stadium kunt u het onderwerpapparaat zien in **de** status In behandeling onder Apparaatblad van Azure Portal.

6. Bij de volgende gebruiker die zich aanmeld bij Windows 10, wordt de registratie voltooid.

    **Opmerking:** Als u VPN gebruikt en aanmelding/aanmelding de domeinconnectiviteit beëindigt, kunt u registratie handmatig activeren. Ga als volgende te werk:
    
    Een lokaal `dsregcmd /join` op beheerdersprompt of op afstand via PSExec op uw pc uitgeven.\
    Bijvoorbeeld:`PsExec -s \\win10client01 cmd, dsregcmd /join`

Zie Veelgestelde vragen over apparaten voor veelvoorkomende problemen met Azure Active Directory [apparaatregistratie.](https://docs.microsoft.com/azure/active-directory/devices/faq)
