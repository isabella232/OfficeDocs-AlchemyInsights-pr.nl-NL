---
title: Problemen met het aanmelden bij Office apps
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938183"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Lege aanmeldingsscherm in Office-toepassingen

U kunt dit probleem oplossen door het volgende proberen:
- Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Opties voor Internet Explorer opnieuw instellen: Ga naar **Extra** > **Internet-opties** > **Geavanceerd** > **Reset Internet Explorer Settings** (Let erop dat u de aangepaste instellingen verliest), en probeer vervolgens het aanmelden bij Office opnieuw.
- Windows Defender-toepassing Guard (WDAG) of een vergelijkbaar programma van de firewall- of antivirusprogramma's uitschakelen:
    1. Ga naar **Software**in het Configuratiescherm en kies vervolgens **Windows-onderdelen in- of uitschakelen**.
    2. Als Windows Defender-toepassing beveiliging is ingeschakeld, schakelt u deze.<br/>
    **Opmerking:** Wellicht moet u de computer opnieuw opstarten.
- Zorg ervoor dat de Microsoft.AAD.BrokerPlugin [AAD WAM-invoegtoepassing](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) niet wordt geblokkeerd door een toepassing of firewall /-virus.
- [Duidelijke Office referenties](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Referentiebeheer.<br/>
    **Opmerking:** De paden voor Office 2016 hebt 16,0 gewijzigd. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Voor meer informatie, Zie [problemen met verbinding bij aanmelden nadat deze is bijgewerkt naar Office 2016 build 16.0.7967 op Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).