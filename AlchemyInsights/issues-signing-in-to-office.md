---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579896"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leeg aanmeldingsscherm in Microsoft 365-apps

Ga als volgt te werk om dit probleem op te lossen:
- Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Explorer-opties opnieuw instellen: ga naar Geavanceerde instellingen **voor het**opnieuw instellen  >  **Internet Options**  >  **van**  >  **Internet Explorer** (houd er rekening mee dat u aangepaste instellingen verliest) en probeer u opnieuw aan te melden bij Office.
- Schakel de Windows Defender Application Guard (WDAG) of een soortgelijke firewall of anti-virus programma uit:
    1. Ga in het Configuratiescherm naar **Programma's**en kies **Windows-functies in- of uitschakelen.**
    2. Als Windows Defender Application Guard is ingeschakeld, probeert u deze uit te schakelen.<br/>
    **Let op:** Mogelijk moet u de computer opnieuw opstarten.
- Zorg ervoor dat de Microsoft.AAD.BrokerPlugin [AAD WAM-plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) niet wordt geblokkeerd door een toepassing of firewall/antivirusprogramma.
- [Office-referenties wissen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met Windows Credential Manager.<br/>
    **Let op:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)

Zie [Verbindingsproblemen in aanmelding na update naar Office 2016 build 16.0.7967 voor](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)meer informatie in Windows 10 .