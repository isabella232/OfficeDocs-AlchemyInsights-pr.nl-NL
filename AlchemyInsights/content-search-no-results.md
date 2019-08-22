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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516774"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="00132-102">Er zijn geen resultaten uit inhoud zoeken-uitvoer</span><span class="sxs-lookup"><span data-stu-id="00132-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="00132-103">Problemen met inhoud zoeken-uitvoer retourneren van gegevens niet kunnen worden veroorzaakt door bepaalde naleving beveiligingsfilter dat is ingesteld door een specifieke Admin en communiceert niet met alle beheerders.</span><span class="sxs-lookup"><span data-stu-id="00132-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="00132-104">U kunt dit oplossen door te controleren op conformiteit beveiligingsfilters die wordt veroorzaakt door dit te controleren:</span><span class="sxs-lookup"><span data-stu-id="00132-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="00132-105">Verbinding maken met de veiligheid en conformiteit Powershell</span><span class="sxs-lookup"><span data-stu-id="00132-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="00132-106">Voer de volgende commandlets:</span><span class="sxs-lookup"><span data-stu-id="00132-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="00132-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="00132-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="00132-108">Get-ComplianceSecurityFilter-$org-organisatie</span><span class="sxs-lookup"><span data-stu-id="00132-108">Get-ComplianceSecurityFilter -Organization $org</span></span>