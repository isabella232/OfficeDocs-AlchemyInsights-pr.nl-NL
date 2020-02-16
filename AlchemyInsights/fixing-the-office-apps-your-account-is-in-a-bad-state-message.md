---
title: De Office-apps herstellen Uw account is in een slecht staatsbericht
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969363"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>De fout van Office-apps 'Uw account is in een slechte staat' herstellen

Als u deze fout wilt oplossen, probeert u de volgende opties op de betreffende computer:

- Open een Office-app en selecteer **Account** > **** > **afmelden van alle accounts**. Meld u opnieuw aan met een gebruikersaccount met een geldige licentie. Zie [Accounts in Office voor](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)meer informatie.
- [Office-referenties wissen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met Windows Credential Manager.<br>
  **Let op:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. \Software\Microsoft\Office\16.0\Common\Identity\
- Stel op de betreffende computer de EnableADAL = 0 in met de volgende stappen:  
     1. Klik met de rechtermuisknop op de knop Windows en selecteer **Uitvoeren**. Typ **regedit**in het vak **Openen** en selecteer **OK**.
     2. Selecteer **Ja** wanneer u wordt gevraagd registereditor toe te staan wijzigingen aan te brengen in uw apparaat.
    3. Voeg in de registereditor een DWORD-waarde van EnableADAL toe met een instelling van 0 onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Als de fout optreedt tijdens het verbinden met Office 365 met Office 2013, [schakelt u moderne verificatie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) in voor de Office-client.

Zie [Problemen met niet-browserapps die zich niet kunnen aanmelden bij Office 365, Azure of Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)voor meer informatie.

