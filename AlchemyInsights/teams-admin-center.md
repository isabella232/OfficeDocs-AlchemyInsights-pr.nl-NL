---
title: Teams-beheercentrum
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826374"
---
# <a name="teams-admin-center"></a>Teams-beheercentrum

Meer informatie over het beheren van Teams met het [Teams-beheercentrum](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Controleer de volgende items als u het Teams-beheercentrum niet kunt openen:

- Controleer dat u de juiste [Office 365 IP-adressen en URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) toestaat op de verbindingsapparaten (firewall, enz.) of in de firewallregels op uw locale machine.
- Controleer of de aanmeldingsgegevens die u gebruikt voor toegang tot het Teams-beheerportaal overeenkomen met uw gebruikersnaam in het [Microsoft 365-beheerportaal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Controleer het volgende als er in het Teams-beheercentrum geen gebruikers worden weergegeven:

- Hebt u in de afgelopen 24 uur gebruikers gemaakt of licenties toegewezen? Wacht minimaal 24 uur voordat u een ondersteuningsticket opent.
- Controleer of u de juiste licenties hebt toegewezen.
- Als u een on-premises Active Directory hebt, controleert u of [de waarde van msRTCSIP-PrimaryUserAddress of het SIP-adres in het veld ProxyAddresses in uw lokale Active Directory uniek is en dat de indeling overeenkomt met](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**gebruikersnaam** van de gebruiker in het [Microsoft 365-beheercentrum](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Als u een implementatie van Skype voor Bedrijven Server wilt behouden en gebruikers on-premises en online wilt hebben, volgt u **Set up hybrid with Teams and Skype for Business Online** (Hybride implementatie met Teams en Skype voor Bedrijven Online instellen) in het Configuratiescherm van Skype voor Bedrijven Server en verplaatst u gebruikers naar online.
