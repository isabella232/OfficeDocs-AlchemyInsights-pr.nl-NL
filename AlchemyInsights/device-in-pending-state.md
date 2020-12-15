---
title: Apparaat met status in behandeling
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677570"
---
# <a name="device-in-pending-state"></a>Apparaat met status in behandeling

**Vereisten**

1. Als u apparaatregistratie voor het eerst instelt, moet u ervoor zorgen dat u de [Inleiding bij Apparaatbeheer hebt bekeken in azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) voor meer informatie over het krijgen van apparaten onder het beheer van Azure AD.
2. Als u apparaten rechtstreeks registreert in azure AD en ze registreert in intune, moet u ervoor zorgen dat u [intune hebt geconfigureerd](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) en de [licenties](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) eerst moet invoeren.
3. Zorg ervoor dat u gemachtigd bent om bewerkingen uit te voeren in azure AD en on-premises AD. U kunt in azure AD alleen een globale beheerder in azure AD instellingen beheren voor apparaatregistratie. Als u automatische registraties in uw on-premises Active Directory wilt instellen, moet u ook een beheerder van Active Directory en AD FS (indien van toepassing) zijn.

Voor het Hybrid Azure AD join-registratieproces zijn apparaten in het bedrijfsnetwerk vereist. Dit werkt ook via VPN, maar er is een aantal voorbehoud. We hebben klanten die u willen assistentie bij het oplossen van problemen met het oplossen van het hybride Azure AD-registratieproces onder externe werkomstandigheden.

**Cloud verificatie omgeving (via Azure AD Password Hash sync of Pass Through-verificatie)**

Deze registratie stroom wordt ook wel ' synchronisatie deelnemen ' genoemd.

Hier ziet u een overzicht van wat er gebeurt tijdens het registratieproces:

1. Windows 10-record service verbindingspunt (SCP) wordt gedetecteerd wanneer de gebruiker zich aanmeldt bij het apparaat.

    1. Het apparaat probeert eerst Tenant informatie op te halen uit de clientzijde-SCP in het register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Zie voor meer informatie [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Als dit mislukt, communiceert het apparaat met on-premises Active Directory om Tenant informatie op te halen van SCP. Als u SCP wilt controleren, raadpleegt u dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > U wordt aangeraden SCP in te schakelen in Active Directory en alleen aan clientzijde-SCP te gebruiken voor de eerste validatie.

2. Windows 10 probeert met Azure AD te communiceren onder de systeemcontext om zichzelf te verifiëren tegen Azure AD.

    U kunt controleren of het apparaat toegang heeft tot Microsoft-bronnen onder het systeemaccount met behulp van het script voor het [registreren van apparaten](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. In Windows 10 wordt zelfondertekend certificaat gegenereerd en opgeslagen onder het computerobject in on-premises Active Directory. Dit vereist regel-van-gezichtsvermogen voor domein controller.

4. Apparaatobject met certificaat dat via Azure AD Connect via Azure AD Connect wordt gesynchroniseerd met Azure AD. De synchronisatie cyclus is standaard elke 30 minuten, maar dit is afhankelijk van de configuratie van Azure AD Connect. Zie dit [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)voor meer informatie.

5. In dit stadium ziet u mogelijk het onderwerp-apparaat in de status **in behandeling** onder apparaatprofielen van Azure Portal.

6. Bij de volgende gebruikersaanmelding met Windows 10 wordt de registratie beëindigd.

    > [!NOTE]
    > Als u gebruikmaakt van VPN en afmelden of als u de domein verbinding beëindigt, kunt u de registratie handmatig activeren. U doet dit als volgt:
    >
    > Meld u aan bij een `dsregcmd /join` lokale beheerder of extern via PSExec op uw PC.
    >
    > Voorbeeld: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Zie [Veelgestelde vragen over apparaten](https://docs.microsoft.com/azure/active-directory/devices/faq)voor algemene problemen met de registratie van Azure Active Directory-apparaten.
