---
title: 1491-Search-Not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776077"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="8399a-102">Zoeken in inhoud niet verwachte resultaten retourneren</span><span class="sxs-lookup"><span data-stu-id="8399a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="8399a-103">Bij het uitvoeren van zoekopdrachten naar de inhoud van het Office 365-beveiliging & conformiteit, wordt u onverwachte resultaten.</span><span class="sxs-lookup"><span data-stu-id="8399a-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="8399a-104">Houd rekening met de volgende dingen die je zoekresultaten kunnen beïnvloeden:</span><span class="sxs-lookup"><span data-stu-id="8399a-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="8399a-105">**Locaties van inhoud en zoekcriteria**: Zorg ervoor dat u de juiste plaats inhoud hebt geselecteerd en zoekcriteria.</span><span class="sxs-lookup"><span data-stu-id="8399a-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="8399a-106">Als u een grote zoekactie (met veel locaties) hebt uitgevoerd, kunt u het opsplitsen in meerdere zoekacties.</span><span class="sxs-lookup"><span data-stu-id="8399a-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="8399a-107">**Gedeeltelijk geïndexeerde items**: [gedeeltelijk geïndexeerde items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) van postbussen zijn opgenomen in de geschatte zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="8399a-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="8399a-108">Echter zijn niet gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive opgenomen in de raming zoeken.</span><span class="sxs-lookup"><span data-stu-id="8399a-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="8399a-109">**Fouten zoeken**: bij het zoeken naar een groot aantal postvakken (meer dan 100.000 postvakken), krijgt u mogelijk fouten zoeken met foutcodes als CS008-009- en CS012-002).</span><span class="sxs-lookup"><span data-stu-id="8399a-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="8399a-110">In dat geval opnieuw proberen de zoekopdracht alleen locaties van de mislukte inhoud.</span><span class="sxs-lookup"><span data-stu-id="8399a-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="8399a-111">Raadpleeg [dit artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8399a-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
