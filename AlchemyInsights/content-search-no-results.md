---
title: Inhoud zoeken zonder resultaten
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816843"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="e8b7e-102">Geen resultaten van Inhoud zoeken/exporteren</span><span class="sxs-lookup"><span data-stu-id="e8b7e-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="e8b7e-103">Problemen met Inhoud zoeken/exporteren die geen gegevens retourneren, kunnen het gevolg zijn van bepaalde compliancebeveiligingsfilters die zijn ingesteld door een specifieke beheerder en die niet aan alle beheerders zijn door te geven.</span><span class="sxs-lookup"><span data-stu-id="e8b7e-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="e8b7e-104">Als u dit wilt oplossen, controleert u of er compliancebeveiligingsfilters zijn die dit kunnen veroorzaken:</span><span class="sxs-lookup"><span data-stu-id="e8b7e-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="e8b7e-105">Verbinding maken met Powershell voor beveiligings- en compliancecentrum</span><span class="sxs-lookup"><span data-stu-id="e8b7e-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e8b7e-106">Voer de volgende opdrachtlets uit:</span><span class="sxs-lookup"><span data-stu-id="e8b7e-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="e8b7e-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="e8b7e-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="e8b7e-108">Get-ComplianceSecurityFilter -Organisatie $org</span><span class="sxs-lookup"><span data-stu-id="e8b7e-108">Get-ComplianceSecurityFilter -Organization $org</span></span>