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
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="e7ab0-102">Het bericht 'Sorry, een ander account van uw organisatie is al aangemeld' herstellen van de Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="e7ab0-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="e7ab0-103">Probeer het volgende om deze fout op te lossen:</span><span class="sxs-lookup"><span data-stu-id="e7ab0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e7ab0-104">Verwijder alle werkaccounts, behalve het betreffende account, met Windows-instellingen > **Toegang tot werk of school.**</span><span class="sxs-lookup"><span data-stu-id="e7ab0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e7ab0-105">[Office-referenties met](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.</span><span class="sxs-lookup"><span data-stu-id="e7ab0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e7ab0-106">**Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="e7ab0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e7ab0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e7ab0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e7ab0-108">Open een Office-app, kies   >  **Bestandsaccount**  >  **uitloggen.** Meld u vervolgens aan met een gebruikersaccount met een geldige licentie.</span><span class="sxs-lookup"><span data-stu-id="e7ab0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e7ab0-109">Zie [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e7ab0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e7ab0-110">Zie voor Mac [Kan me niet aanmelden bij een Office 2016 voor Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e7ab0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="e7ab0-111">Zie 'Sorry, een ander account van uw organisatie is al aangemeld [op deze computer' in Office voor meer informatie.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="e7ab0-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>