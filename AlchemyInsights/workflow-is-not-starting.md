---
title: Werkstroom wordt niet gestart
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766092"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="49632-102">Werkstroom wordt niet gestart</span><span class="sxs-lookup"><span data-stu-id="49632-102">Workflow is not starting</span></span>

- <span data-ttu-id="49632-103">SharePoint 2010- en SharePoint 2013-werkstromen worden niet gestart.</span><span class="sxs-lookup"><span data-stu-id="49632-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="49632-104">Als uw werkstroom niet wordt gestart, kan er een tijdelijke serviceprobleem zijn waarbij gebruikers met tussenpozen vertragingen kunnen ondervinden bij de voortgang van de werkstroom.</span><span class="sxs-lookup"><span data-stu-id="49632-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="49632-105">Controleer het [dashboard servicestatus](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of de impact van uw organisatie is.</span><span class="sxs-lookup"><span data-stu-id="49632-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="49632-106">Als er meer dan 24 uur zijn verstreken sinds je dit probleem voor het eerst zag, log dan een ondersteuningsticket in.</span><span class="sxs-lookup"><span data-stu-id="49632-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="49632-107">In veel gevallen werken we al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="49632-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="49632-108">Geef ons minstens 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="49632-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="49632-109">SharePoint 2010-werkstromen vertraagd bij het starten.</span><span class="sxs-lookup"><span data-stu-id="49632-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="49632-110">Dit gebeurt als de werkstroom in grote batches wordt geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="49632-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="49632-111">(bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).</span><span class="sxs-lookup"><span data-stu-id="49632-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="49632-112">Werkstromen zijn niet ontworpen om real-time uit te voeren, dus een vertraging is het ontwerpgedrag.</span><span class="sxs-lookup"><span data-stu-id="49632-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="49632-113">Als de werkstroom complexe Extensible Object Markup Language (XMOL) is, kan de compilatie traag zijn.</span><span class="sxs-lookup"><span data-stu-id="49632-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="49632-114">Check [dit](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="49632-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="49632-115">U moet de werkstroom vereenvoudigen of opnieuw ontwerpen met het type Microsoft SharePoint 2013-werkstroomplatform.</span><span class="sxs-lookup"><span data-stu-id="49632-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="49632-116">Als uw werkstroomgeschiedenis groot is geworden, u de items verwijderen of een nieuwe geschiedenislijst maken.</span><span class="sxs-lookup"><span data-stu-id="49632-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="49632-117">Meer informatie : [Werkstroomgeschiedenis wissen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="49632-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="49632-118">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="49632-118">Related topics</span></span>
<span data-ttu-id="49632-119">Wilt u Microsoft Flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="49632-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="49632-120">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="49632-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="49632-121">SharePoint en Flow</span><span class="sxs-lookup"><span data-stu-id="49632-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


