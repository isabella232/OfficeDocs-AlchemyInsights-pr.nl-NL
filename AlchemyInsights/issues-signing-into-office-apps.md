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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579860"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Het bericht microsoft 365-apps 'De trusted platformmodule van uw computer werkt niet goed' herstellen

Probeer het volgende om deze fout op te lossen:

- Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Office-referenties wissen](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met Windows Credential Manager.<br/>
    **Let op:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)
- Probeer het [herstelproces van](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) de gebruiker om TPM-fouten (Trusted Platform Module) op te lossen.
- Stel de EnableADAL = 0 in met de volgende stappen:  
    1. Klik met de rechtermuisknop op de knop Start van Windows, kies **Uitvoeren**, typ **regedit**en kies **OK**.
    2. Selecteer **Ja** om registereditor toe te staan wijzigingen aan te brengen in uw apparaat.
    3. Voeg in registereditor een DWORD-waarde van **EnableADAL** toe met een instelling van **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Zie [Verbindingsproblemen in aanmelding na update naar Office 2016 build 16.0.7967 voor](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)meer informatie in Windows 10 .