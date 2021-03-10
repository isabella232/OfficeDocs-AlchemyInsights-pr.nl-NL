---
title: Best practices toepassen voor geavanceerde zoekquery's
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693346"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="e743a-102">Best practices toepassen voor geavanceerde zoekquery's</span><span class="sxs-lookup"><span data-stu-id="e743a-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="e743a-103">Als u sneller resultaten wilt krijgen en time-outs wilt vermijden tijdens het uitvoeren van complexe query's, moet u de volgende best practices toepassen:</span><span class="sxs-lookup"><span data-stu-id="e743a-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="e743a-104">Wanneer u nieuwe query's probeert, moet u altijd een limiet gebruiken om te voorkomen dat u zeer grote resultatensets krijgt.</span><span class="sxs-lookup"><span data-stu-id="e743a-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="e743a-105">Gebruik deze optie ook om een eerste evaluatie te maken van de grootte `count` van de resultatenset.</span><span class="sxs-lookup"><span data-stu-id="e743a-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="e743a-106">Gebruik eerst tijdfilters.</span><span class="sxs-lookup"><span data-stu-id="e743a-106">Use time filters first.</span></span> <span data-ttu-id="e743a-107">Beperk uw query's het beste tot zeven dagen.</span><span class="sxs-lookup"><span data-stu-id="e743a-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="e743a-108">Aan het begin van een query, direct na het tijdfilter, voegt u de filters toe die de meeste gegevens naar verwachting zullen verwijderen.</span><span class="sxs-lookup"><span data-stu-id="e743a-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="e743a-109">Als u op zoek bent naar volledige tokens, gebruikt u de `has` operator in plaats van `contains` .</span><span class="sxs-lookup"><span data-stu-id="e743a-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="e743a-110">Voer een zoekopdracht uit op een specifieke kolom in plaats van voor alle kolommen.</span><span class="sxs-lookup"><span data-stu-id="e743a-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="e743a-111">Wanneer u tabellen wilt samenvoegen, geeft u eerst de tabel met minder rijen op.</span><span class="sxs-lookup"><span data-stu-id="e743a-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="e743a-112">`project` alleen de benodigde kolommen uit de tabellen die u hebt samengevoegd.</span><span class="sxs-lookup"><span data-stu-id="e743a-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="e743a-113">Zie geavanceerde [zoekquery-best practices voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="e743a-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
