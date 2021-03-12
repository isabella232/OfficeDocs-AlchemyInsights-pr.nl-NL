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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744607"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="0d5db-102">Best practices toepassen voor geavanceerde zoekquery's</span><span class="sxs-lookup"><span data-stu-id="0d5db-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="0d5db-103">Als u sneller resultaten wilt boeken en time-outs wilt vermijden tijdens het uitvoeren van complexe query's, past u de volgende best practices toe:</span><span class="sxs-lookup"><span data-stu-id="0d5db-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="0d5db-104">Wanneer u nieuwe query's probeert, gebruikt u altijd een limiet om te voorkomen dat u zeer grote resultatensets krijgt.</span><span class="sxs-lookup"><span data-stu-id="0d5db-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="0d5db-105">Gebruik deze optie ook om een eerste beoordeling te maken van de grootte van `count` de resultatenset.</span><span class="sxs-lookup"><span data-stu-id="0d5db-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="0d5db-106">Gebruik eerst tijdfilters.</span><span class="sxs-lookup"><span data-stu-id="0d5db-106">Use time filters first.</span></span> <span data-ttu-id="0d5db-107">Beperk uw query's in het ideale ideaal tot zeven dagen.</span><span class="sxs-lookup"><span data-stu-id="0d5db-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="0d5db-108">Voeg aan het begin van een query, direct na het tijdfilter, de filters toe die naar verwachting de meeste gegevens zullen verwijderen.</span><span class="sxs-lookup"><span data-stu-id="0d5db-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="0d5db-109">Wanneer u op zoek bent naar volledige tokens, gebruikt u de `has` operator in plaats van `contains` .</span><span class="sxs-lookup"><span data-stu-id="0d5db-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="0d5db-110">Voer een zoekopdracht uit in een specifieke kolom in plaats van in alle kolommen.</span><span class="sxs-lookup"><span data-stu-id="0d5db-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="0d5db-111">Geef bij het deelnemen aan tabellen eerst de tabel op met minder rijen.</span><span class="sxs-lookup"><span data-stu-id="0d5db-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="0d5db-112">`project` alleen de benodigde kolommen uit de tabellen die u hebt samengevoegd.</span><span class="sxs-lookup"><span data-stu-id="0d5db-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="0d5db-113">Zie Geavanceerde best practices [voor query's voor query's voor geavanceerde query's voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="0d5db-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
