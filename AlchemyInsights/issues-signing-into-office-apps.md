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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695174"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Het repareren van de Microsoft 365-apps "de vertrouwde platform module van uw computer functioneert niet goed"

Probeer het volgende om deze fout op te lossen:

- Installeer de meest recente updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Wis Office-referenties](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Credential Manager.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16,0. (Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)
- Probeer het [gebruikersherstel proces](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) voor het oplossen van TPM-fouten (Trusted Platform Module).
- Stel de EnableADAL = 0 in met de volgende stappen:  
    1. Klik met de rechtermuisknop op de knop Start van Windows, kies **uitvoeren**, typ **regedit**en klik vervolgens op **OK**.
    2. Selecteer **Ja** als u wilt dat de Register-editor wijzigingen aan uw apparaat aanbrengt.
    3. In de Register-editor voegt u de DWORD-waarde **EnableADAL** met de instelling **0** onder HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Zie voor meer informatie [verbindingsproblemen tijdens het aanmelden na update naar Office 2016 build 16.0.7967 voor Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).