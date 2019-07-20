---
title: Inhoud zoeken geen resultaten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800282"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="f0f62-102">Er zijn geen resultaten uit inhoud zoeken-uitvoer</span><span class="sxs-lookup"><span data-stu-id="f0f62-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="f0f62-103">Problemen met inhoud zoeken-uitvoer retourneren van gegevens niet kunnen worden veroorzaakt door bepaalde naleving beveiligingsfilter dat is ingesteld door een specifieke Admin en communiceert niet met alle beheerders.</span><span class="sxs-lookup"><span data-stu-id="f0f62-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="f0f62-104">U kunt dit oplossen door te controleren op conformiteit beveiligingsfilters die wordt veroorzaakt door dit te controleren:</span><span class="sxs-lookup"><span data-stu-id="f0f62-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="f0f62-105">Verbinding maken met de veiligheid en conformiteit Powershell</span><span class="sxs-lookup"><span data-stu-id="f0f62-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f0f62-106">Voer de volgende commandlets:</span><span class="sxs-lookup"><span data-stu-id="f0f62-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="f0f62-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="f0f62-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="f0f62-108">Get-ComplianceSecurityFilter-$org-organisatie</span><span class="sxs-lookup"><span data-stu-id="f0f62-108">Get-ComplianceSecurityFilter -Organization $org</span></span>