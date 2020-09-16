---
title: 1491-zoeken met niet-verwachte resultaten-resultaten
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740469"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d5724-102">Inhouds zoekactie levert geen verwachte resultaten op</span><span class="sxs-lookup"><span data-stu-id="d5724-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d5724-103">Wanneer u inhouds zoekopdrachten uitvoert vanuit het compliance-beveiligings & van Microsoft 365, krijgt u mogelijk onverwachte zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="d5724-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d5724-104">Houd rekening met de volgende dingen die van invloed kunnen zijn op de zoekresultaten:</span><span class="sxs-lookup"><span data-stu-id="d5724-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d5724-105">**Inhoudslocaties en zoekvoorwaarden**: Zorg ervoor dat u de juiste inhoudslocaties en zoekvoorwaarden hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="d5724-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d5724-106">Als u een grote zoekopdracht met een groot aantal locaties hebt uitgevoerd, kunt u deze in meerdere zoekopdrachten verdelen.</span><span class="sxs-lookup"><span data-stu-id="d5724-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d5724-107">**Gedeeltelijk geïndexeerde items**:  [gedeeltelijk geïndexeerde items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) uit postvakken worden opgenomen in de geschatte zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="d5724-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d5724-108">Gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive worden echter niet opgenomen in de zoek raming.</span><span class="sxs-lookup"><span data-stu-id="d5724-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d5724-109">**Zoek fouten**: bij het zoeken in een groot aantal postvakken (meer dan 100.000 postvakken), worden mogelijk Zoek fouten weergegeven, met foutcodes zoals CS008-009 en CS012-002.</span><span class="sxs-lookup"><span data-stu-id="d5724-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d5724-110">In dit geval kunt u de zoekfunctie alleen opnieuw uitvoeren voor de mislukte inhoudslocaties.</span><span class="sxs-lookup"><span data-stu-id="d5724-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d5724-111">Zie  [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d5724-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
