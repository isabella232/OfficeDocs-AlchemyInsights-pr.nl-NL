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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833070"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Het bericht 'Sorry, een ander account van uw organisatie is al aangemeld' herstellen van de Microsoft 365-apps

Probeer het volgende om deze fout op te lossen:

- Verwijder alle werkaccounts, behalve het betreffende account, met Windows-instellingen > **Toegang tot werk of school.**
- [Office-referenties met](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.<br/>
    **Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Open een Office-app, kies   >  **Bestandsaccount**  >  **uitloggen.** Meld u vervolgens aan met een gebruikersaccount met een geldige licentie. Zie [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) voor meer informatie.
- Zie voor Mac [Kan me niet aanmelden bij een Office 2016 voor Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Zie 'Sorry, een ander account van uw organisatie is al aangemeld [op deze computer' in Office voor meer informatie.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)