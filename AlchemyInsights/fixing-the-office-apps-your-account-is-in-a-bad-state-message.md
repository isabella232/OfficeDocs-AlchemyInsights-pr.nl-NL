---
title: De Microsoft 365-apps herstellen die het bericht heeft over een onjuiste status
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744540"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>De foutmelding over het herstellen van de Microsoft 365-apps "uw account is beschadigd"

U kunt deze fout oplossen met de volgende opties op de desbetreffende computer:

- Open een Office-app en **Selecteer**  >  **Account**  >  **Afmelden bij het account van alle accounts**. Meld u opnieuw aan met een gebruikersaccount met een geldige licentie. Zie [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) voor meer informatie.
- [Wis Office-referenties](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Credential Manager.<br>
  **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16,0. Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\
- Als de fout optreedt tijdens het maken van verbinding met Office 365 met behulp van Office 2013, [schakelt u moderne verificatie in](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) voor de Office-client.

Voor meer informatie raadpleegt [u problemen met niet-browser-apps oplossen waarmee u zich niet kunt aanmelden bij Microsoft 365, Azure of intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

