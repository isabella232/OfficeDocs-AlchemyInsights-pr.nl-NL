---
title: 1491-search-not-return-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709222"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="451b1-102">Content Search levert geen verwachte resultaten op</span><span class="sxs-lookup"><span data-stu-id="451b1-102">Content Search not returning expected results</span></span>

<span data-ttu-id="451b1-103">Wanneer u inhoudszoekopdrachten uitvoert vanuit het Microsoft 365-beveiligingscentrum & Compliance Center, ontvangt u mogelijk onverwachte zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="451b1-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="451b1-104">Houd rekening met de volgende dingen die van invloed kunnen zijn op uw zoekresultaten:</span><span class="sxs-lookup"><span data-stu-id="451b1-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="451b1-105">**Inhoudslocaties en zoekomstandigheden:** zorg ervoor dat u de juiste inhoudslocaties en zoekomstandigheden hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="451b1-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="451b1-106">Als u een grote zoekopdracht hebt uitgevoerd (met veel locaties), u overwegen deze op te splitsen in meerdere zoekopdrachten.</span><span class="sxs-lookup"><span data-stu-id="451b1-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="451b1-107">**Gedeeltelijk geïndexeerde items**: [Gedeeltelijk geïndexeerde items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) uit postvakken worden opgenomen in de geschatte zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="451b1-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="451b1-108">Gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive worden echter niet opgenomen in de zoekschatting.</span><span class="sxs-lookup"><span data-stu-id="451b1-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="451b1-109">**Zoekfouten**: Bij het doorzoeken van een groot aantal postvakken (meer dan 100.000 postvakken) u zoekfouten krijgen, met foutcodes zoals CS008-009 en CS012-002).</span><span class="sxs-lookup"><span data-stu-id="451b1-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="451b1-110">Probeer in dit geval de zoekopdracht alleen opnieuw naar de mislukte inhoudslocaties.</span><span class="sxs-lookup"><span data-stu-id="451b1-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="451b1-111">Zie [dit artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="451b1-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
