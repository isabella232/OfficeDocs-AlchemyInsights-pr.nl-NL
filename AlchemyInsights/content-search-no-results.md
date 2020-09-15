---
title: Inhoud zoeken geen resultaten
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680642"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="257e5-102">Geen resultaten van inhouds zoekactie/-uitvoer</span><span class="sxs-lookup"><span data-stu-id="257e5-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="257e5-103">Problemen bij het zoeken naar inhoud en exporteren van inhoud kan worden veroorzaakt door een bepaald nalevings beveiligings filter dat door een specifieke beheerder is ingesteld en de communicatie met de beheerder niet naar alle beheerders hoeft te communiceren.</span><span class="sxs-lookup"><span data-stu-id="257e5-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="257e5-104">U kunt dit oplossen door te controleren of er beveiligings filters voor compliance zijn die dit mogelijk veroorzaken:</span><span class="sxs-lookup"><span data-stu-id="257e5-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="257e5-105">Verbinding maken met PowerShell van Beveiligingscentrum en compliance</span><span class="sxs-lookup"><span data-stu-id="257e5-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="257e5-106">Voer de volgende Commandlets:</span><span class="sxs-lookup"><span data-stu-id="257e5-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="257e5-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="257e5-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="257e5-108">Get-ComplianceSecurityFilter-organisatie $org</span><span class="sxs-lookup"><span data-stu-id="257e5-108">Get-ComplianceSecurityFilter -Organization $org</span></span>