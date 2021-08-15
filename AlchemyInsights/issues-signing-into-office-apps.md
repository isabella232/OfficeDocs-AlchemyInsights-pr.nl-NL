---
title: Problemen met het aanmelden bij Microsoft 365 apps
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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986886"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Het oplossen Microsoft 365 apps 'De vertrouwde platformmodule van uw computer werkt niet goed' bericht

Probeer het volgende om deze fout op te lossen:

- Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [U Office referenties met Windows](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Credential Manager.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Probeer het [herstelproces voor gebruikers om](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-fouten (Trusted Platform Module) op te lossen.
- Stel enableADAL = 0 in met de volgende stappen:  
    1. Klik met de rechtermuisknop op Windows startknop, kies **Uitvoeren,** typ **regedit** en kies **OK.**
    2. Selecteer **Ja** om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.
    3. Voeg in registereditor een DWORD-waarde van **EnableADAL** toe met een instelling **van 0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Zie Verbindingsproblemen in aanmelding na update naar [Office 2016 build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)op Windows 10.