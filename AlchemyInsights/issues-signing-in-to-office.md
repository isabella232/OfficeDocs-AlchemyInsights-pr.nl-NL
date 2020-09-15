---
title: Problemen bij het aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695282"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leeg aanmeldingsscherm in Microsoft 365-apps

Probeer het volgende om dit probleem op te lossen:
- Installeer de meest recente updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Opties voor Internet Explorer opnieuw instellen: Ga naar **extra**  >  **Internetopties**  >  **Geavanceerde**  >  **instellingen voor Internet Explorer herstellen** (u verliest aangepaste instellingen) en probeer u vervolgens opnieuw aan te melden bij Office.
- Schakel de Windows Defender Application Guard (WDAG) of een soortgelijke firewall-of antivirusprogramma van derden uit:
    1. Ga in het Configuratiescherm naar **Programma's**en kies vervolgens **Windows-functies in-of uitschakelen**.
    2. Als Windows Defender Application Guard is ingeschakeld, kunt u dit uitschakelen.<br/>
    **Opmerking:** Mogelijk moet u de computer opnieuw opstarten.
- Zorg ervoor dat de [Aad WAM-invoeg](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) toepassing van Microsoft. Aad. BrokerPlugin niet wordt geblokkeerd door een toepassing of een ander anti-virusprogramma.
- [Wis Office-referenties](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Credential Manager.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16,0. (Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)

Zie voor meer informatie [verbindingsproblemen tijdens het aanmelden na update naar Office 2016 build 16.0.7967 voor Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).