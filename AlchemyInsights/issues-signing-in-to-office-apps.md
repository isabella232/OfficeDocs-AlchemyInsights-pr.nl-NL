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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695318"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Bericht over het repareren van de Microsoft 365-apps ' Sorry, er is al een ander account van uw organisatie is aangemeld '

Probeer het volgende om deze fout op te lossen:

- Verwijder alle werk accounts, met uitzondering van het betreffende account, met behulp van Windows-instellingen > **toegang tot werk of school**.
- [Wis Office-referenties](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Credential Manager.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16,0. (Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)
- Open een Office-app, kies **Bestands**  >  **account**  >  **Afmelden**. Meld u vervolgens aan met een gebruikersaccount met een geldige licentie. Zie [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) voor meer informatie.
- Zie voor Mac [Kan me niet aanmelden bij een Office 2016 voor Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Zie voor meer informatie [een ander account van uw organisatie is al aangemeld op deze computer in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).