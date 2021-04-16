---
title: eDiscovery-exporthulpmiddel
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814583"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="13136-102">Kunt u het eDiscovery-exportprogramma niet installeren of uitvoeren?</span><span class="sxs-lookup"><span data-stu-id="13136-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="13136-103">Als u het eDiscovery-exportprogramma niet kunt installeren of uitvoeren om zoekresultaten te downloaden, controleert u de volgende dingen:</span><span class="sxs-lookup"><span data-stu-id="13136-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="13136-104">De computer die u gebruikt, voldoet aan de volgende vereisten:</span><span class="sxs-lookup"><span data-stu-id="13136-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="13136-105">32- of 64-bits versies van Windows 7 en nieuwere versies</span><span class="sxs-lookup"><span data-stu-id="13136-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="13136-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="13136-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="13136-107">Een ondersteunde browser:</span><span class="sxs-lookup"><span data-stu-id="13136-107">A supported browser:</span></span>

  - <span data-ttu-id="13136-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="13136-108">Microsoft Edge</span></span>

    <span data-ttu-id="13136-109">Of</span><span class="sxs-lookup"><span data-stu-id="13136-109">Or</span></span>

  - <span data-ttu-id="13136-110">Internet Explorer 10 en nieuwere versies</span><span class="sxs-lookup"><span data-stu-id="13136-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="13136-111">Andere browsers, zoals Google Chrome en Mozilla Firefox, worden niet ondersteund.</span><span class="sxs-lookup"><span data-stu-id="13136-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="13136-112">Uw organisatie kan verbinding maken met het eindpunt in Azure, dat **\* .blob.core.windows.net** is (het jokerteken vertegenwoordigt een unieke id voor uw exportklus).</span><span class="sxs-lookup"><span data-stu-id="13136-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="13136-113">U krijgt de rol Exporteren toegewezen in het Microsoft 365 Security &amp; Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="13136-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="13136-114">Deze rol wordt standaard alleen toegewezen aan de rollengroep eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="13136-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="13136-115">Zie [EDiscovery-machtigingen toewijzen.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="13136-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="13136-116">Zie Inhoudszoekresultaten [exporteren voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="13136-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="13136-117">Als u meer dan 100.000 postvakken exporteert, moet u de volgende Powershell gebruiken om de exportresultaten te downloaden: Resultaten exporteren uit meer dan [100.000 postvakken.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="13136-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>