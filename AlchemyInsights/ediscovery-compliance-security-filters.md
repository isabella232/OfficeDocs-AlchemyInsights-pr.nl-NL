---
title: Geen resultaten geretourneerd tijdens het zoeken naar inhoud en exporteren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677682"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="63d60-102">Geen resultaten geretourneerd tijdens het zoeken naar inhoud en exporteren</span><span class="sxs-lookup"><span data-stu-id="63d60-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="63d60-103">Als u problemen ondervindt met de volgende eDiscovery-scenario's:</span><span class="sxs-lookup"><span data-stu-id="63d60-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="63d60-104">Inhoud zoeken/exporteren geeft geen gegevens of onverwachte gegevens als resultaat</span><span class="sxs-lookup"><span data-stu-id="63d60-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="63d60-105">eDiscovery-zoekopdrachten of exporteren mislukt</span><span class="sxs-lookup"><span data-stu-id="63d60-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="63d60-106">Dit kan gebeuren vanwege beveiligings filters voor naleving die door een bepaalde beheerder zijn ingesteld en die niet zijn gecommuniceerd aan alle beheerders.</span><span class="sxs-lookup"><span data-stu-id="63d60-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="63d60-107">U kunt dit oplossen door te controleren of er beveiligings filters voor naleving zijn die deze problemen mogelijk veroorzaken:</span><span class="sxs-lookup"><span data-stu-id="63d60-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="63d60-108">Verbinding maken met PowerShell van Beveiligingscentrum en compliance</span><span class="sxs-lookup"><span data-stu-id="63d60-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="63d60-109">Voer de volgende Commandlets:</span><span class="sxs-lookup"><span data-stu-id="63d60-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="63d60-110">Zie voor meer informatie over beveiligings filters voor naleving de [machtigingen filters voor inhoud zoeken](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="63d60-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
