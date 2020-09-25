---
title: hulpprogramma voor het exporteren van eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277931"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="f764d-102">Kunt u het hulpprogramma voor het maken van eDiscovery-export niet installeren of uitvoeren?</span><span class="sxs-lookup"><span data-stu-id="f764d-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="f764d-103">Controleer het volgende als u het hulpprogramma voor het maken van zoekresultaten niet kunt installeren of uitvoeren voor het gebruik van het hulpprogramma eDiscovery-export.</span><span class="sxs-lookup"><span data-stu-id="f764d-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="f764d-104">De computer die u gebruikt voldoet aan de volgende vereisten:</span><span class="sxs-lookup"><span data-stu-id="f764d-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="f764d-105">32-of 64-bits versies van Windows 7 en nieuwere versies</span><span class="sxs-lookup"><span data-stu-id="f764d-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="f764d-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="f764d-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="f764d-107">Een ondersteunde browser:</span><span class="sxs-lookup"><span data-stu-id="f764d-107">A supported browser:</span></span>

  - <span data-ttu-id="f764d-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f764d-108">Microsoft Edge</span></span>

    <span data-ttu-id="f764d-109">Of</span><span class="sxs-lookup"><span data-stu-id="f764d-109">Or</span></span>

  - <span data-ttu-id="f764d-110">Internet Explorer 10 en nieuwere versies</span><span class="sxs-lookup"><span data-stu-id="f764d-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="f764d-111">Andere browsers zoals Google Chrome en Mozilla Firefox worden niet ondersteund.</span><span class="sxs-lookup"><span data-stu-id="f764d-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="f764d-112">Uw organisatie kan verbinding maken met het eindpunt in azure, dat wil zeggen \*\* \* . blob.core.Windows.net\*\* (het jokerteken vertegenwoordigt een unieke id voor de exporttaak).</span><span class="sxs-lookup"><span data-stu-id="f764d-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="f764d-113">U bent in het Microsoft 365 beveiligings compliance van de export functie toegewezen &amp; .</span><span class="sxs-lookup"><span data-stu-id="f764d-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="f764d-114">Standaard is deze rol alleen toegewezen aan de rollen groep van eDiscovery-beheerders.</span><span class="sxs-lookup"><span data-stu-id="f764d-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="f764d-115">Zie [eDiscovery-machtigingen toewijzen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="f764d-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="f764d-116">Zie [inhoud van zoekresultaten exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f764d-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="f764d-117">Als u meer dan een afgesloten 100k postvakken exporteert, moet u de volgende PowerShell gebruiken om de export resultaten te downloaden:  [resultaten uit meer dan afgesloten 100k postvakken exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="f764d-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>