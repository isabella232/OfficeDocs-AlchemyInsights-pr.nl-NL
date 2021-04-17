---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833026"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leeg aanmeldingsscherm in Microsoft 365-apps

Probeer het volgende om dit probleem op te lossen:
- Installeer de meest recente updates [voor Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Opties voor Internet Explorer opnieuw instellen: Ga naar **Hulpprogramma's**  >  **Internetopties** Geavanceerd  >    >  **Internet Explorer-instellingen** opnieuw instellen (houd er rekening mee dat aangepaste instellingen verloren gaan) en probeer u opnieuw aan te melden bij Office.
- Schakel de Windows Defender Application Guard (WDAG) of een soortgelijk firewall- of antivirusprogramma uit:
    1. Ga in het Configuratiescherm naar **Programma's** en kies **Vervolgens Windows-functies in- of uitschakelen.**
    2. Als Windows Defender Application Guard is ingeschakeld, kunt u deze uitschakelen.<br/>
    **Opmerking:** Mogelijk moet u de computer opnieuw opstarten.
- Zorg ervoor dat de Microsoft.AAD.MakelaarPlugin [AAD WAM-insteektoepassing](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) niet wordt geblokkeerd door een toepassing of firewall/anti-virusprogramma.
- [Office-referenties met](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Zie Verbindingsproblemen in aanmelding na update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.