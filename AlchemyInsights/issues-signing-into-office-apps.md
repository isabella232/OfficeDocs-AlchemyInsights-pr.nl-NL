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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832998"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Het bericht 'De vertrouwde platformmodule van uw computer werkt niet goed' van de Microsoft 365-apps herstellen

Probeer het volgende om deze fout op te lossen:

- Installeer de meest recente updates [voor Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Office-referenties met](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Probeer het [herstelproces voor gebruikers om](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-fouten (Trusted Platform Module) op te lossen.
- Stel enableADAL = 0 in met de volgende stappen:  
    1. Klik met de rechtermuisknop op de knop Start van Windows, **kies Uitvoeren,** typ **regedit** en kies **OK.**
    2. Selecteer **Ja** om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.
    3. Voeg in registereditor een DWORD-waarde van **EnableADAL** toe met een instelling **van 0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Zie Verbindingsproblemen in aanmelding na update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.