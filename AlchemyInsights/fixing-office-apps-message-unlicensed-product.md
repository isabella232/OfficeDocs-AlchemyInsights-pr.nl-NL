---
title: Office kan niet worden geactiveerd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704925"
---
# <a name="unable-to-activate-office"></a>Office kan niet worden geactiveerd

- Controleer of de status van het abonnement is verlopen.
- Zorg ervoor dat je een-abonnement hebt waarvoor client-licenties zijn toegestaan, zoals Office 365 Business of Business Premium en [zorg ervoor dat de gebruiker een licentie toegewezen heeft gekregen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Zorg ervoor dat de gebruiker zich bij Office aanmeldt met hetzelfde account waaraan de licentie is toegewezen.
- Raadpleeg de [pagina voor de Office 365-servicestatus](https://docs.microsoft.com/office365/enterprise/view-service-health) om te zien of er bekende problemen zijn met de service.
- Controleer de firewall, de antivirussoftware en de proxyinstellingen om te bevestigen dat deze de toegang van Microsoft 365-apps tot internet niet blokkeren. Zie [URL's en IP-adresbereiken voor Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL's en IP-adresbereiken").

**Tip** op Windows-machines kunnen verschillende algemene problemen met aanmelden bij Office geconstateerd en automatisch opgelost worden. Download en voer de **[Microsoft Ondersteunings- en herstelassistent](https://aka.ms/SaRA-OfficeSignInScenario)** uit om het automatische hulpprogramma te gebruiken.

Gebruik de volgende acties voor het oplossen van problemen:

- Open een Office-app en [meld u af](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bij bestaande gebruikersaccounts. [Verwijder](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) de Office-licentie en [wijs deze opnieuw toe](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users). Vervolgens [meldt u zich aan bij Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) met het desbetreffende gebruikersaccount.
- De [probleemoplosser voor de activering](https://aka.ms/SARA-OfficeActivation-Alchemy) uitvoeren
- [Activeringsstatus van Office opnieuw instellen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Activeringsstatus van Office opnieuw instellen")
- [Onlineherstel van Office uitvoeren](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Zie voor extra oplossingen voor het oplossen van problemen:  

- [Fouten met producten zonder licentie en activeringsfouten in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Fout 'Er kan geen verbinding worden gemaakt met uw account. Probeer het later opnieuw' bij het activeren van Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)