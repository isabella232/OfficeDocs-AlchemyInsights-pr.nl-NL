---
title: Problemen met aanmelden bij Microsoft 365-apps
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709101"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fix the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message

Probeer het volgende om deze fout op te lossen:

- Installeer de meest recente updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Office-referenties leeg te maken](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) met Windows Referentiebeheer.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Probeer het [gebruikersherstelproces om](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) fouten in de TPM (Trusted Platform Module) op te lossen.
- Stel enableADAL = 0 in door de volgende stappen uit te voeren:  
    1. Klik met de rechtermuisknop op de startknop van Windows, kies **Uitvoeren,** typ **regedit** en kies **OK.**
    2. Selecteer **Ja om** toe te staan dat de Register-editor wijzigingen aan uw apparaat aan kan brengen.
    3. Voeg in de Register-editor de DWORD-waarde van **EnableADAL** toe met de instelling **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Zie Verbindingsproblemen bij het aanmelden na een update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.