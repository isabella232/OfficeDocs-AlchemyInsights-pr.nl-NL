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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938184"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Tot vaststelling van het bericht Office apps 'vertrouwde Platform-module van de computer niet goed werkt. "

U kunt deze fout oplossen door het volgende proberen:

- Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Duidelijke Office referenties](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Referentiebeheer.<br/>
    **Opmerking:** De paden voor Office 2016 hebt 16,0 gewijzigd. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Voer het [herstelproces gebruiker](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) u Trusted Platform Module (TPM)-fouten kunt oplossen.
- Stel de EnableADAL = 0, met behulp van de volgende stappen uit:  
    1. Klik met de rechtermuisknop op de knop Start, kies **uitvoeren**, typ **regedit**en klik op **OK**.
    2. Selecteer **Ja** om de Register-Editor om uw apparaat te wijzigen.
    3. In de Register-Editor een DWORD-waarde van **EnableADAL** met een instelling van **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity toevoegen

Voor meer informatie, Zie [problemen met verbinding bij aanmelden nadat deze is bijgewerkt naar Office 2016 build 16.0.7967 op Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).