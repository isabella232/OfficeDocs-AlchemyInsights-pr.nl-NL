---
title: De werkstroom wordt niet gestart
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738084"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="49d6f-102">De werkstroom wordt niet gestart</span><span class="sxs-lookup"><span data-stu-id="49d6f-102">Workflow is not starting</span></span>

- <span data-ttu-id="49d6f-103">SharePoint 2010 en SharePoint 2013 werkstromen worden niet gestart.</span><span class="sxs-lookup"><span data-stu-id="49d6f-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="49d6f-104">Als uw werkstroom niet wordt gestart, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers periodieke vertragingen met workflowvoortgang kunnen ondervinden.</span><span class="sxs-lookup"><span data-stu-id="49d6f-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="49d6f-105">Controleer de [service status dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie wordt beïnvloed.</span><span class="sxs-lookup"><span data-stu-id="49d6f-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="49d6f-106">Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst zag, logt u een ondersteuningsticket in.</span><span class="sxs-lookup"><span data-stu-id="49d6f-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="49d6f-107">In veel gevallen werken we nu al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="49d6f-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="49d6f-108">Gelieve ons ten minste 24 uur te geven om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="49d6f-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="49d6f-109">SharePoint 2010 werkstromen vertraagd bij het starten.</span><span class="sxs-lookup"><span data-stu-id="49d6f-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="49d6f-110">Dit gebeurt als de werkstroom wordt geactiveerd in grote batches.</span><span class="sxs-lookup"><span data-stu-id="49d6f-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="49d6f-111">(bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).</span><span class="sxs-lookup"><span data-stu-id="49d6f-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="49d6f-112">Workflows zijn niet ontworpen om real-time uit te voeren, dus een vertraging is per ontwerp gedrag.</span><span class="sxs-lookup"><span data-stu-id="49d6f-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="49d6f-113">Als de werkstroom complexe Extensible object Markup Language (XMOL) is, kan compilatie traag zijn.</span><span class="sxs-lookup"><span data-stu-id="49d6f-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="49d6f-114">Raadpleeg [Dit](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="49d6f-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="49d6f-115">U moet de werkstroom vereenvoudigen of opnieuw ontwerpen met het type werkstroom platform van Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="49d6f-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="49d6f-116">Als de werkstroomgeschiedenis groot is gegroeid, u de items verwijderen of een nieuwe geschiedenislijst maken.</span><span class="sxs-lookup"><span data-stu-id="49d6f-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="49d6f-117">Meer informatie: [Workflowhistorie opschonen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="49d6f-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="49d6f-118">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="49d6f-118">Related topics</span></span>
<span data-ttu-id="49d6f-119">Wilt u Microsoft flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="49d6f-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="49d6f-120">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="49d6f-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="49d6f-121">SharePoint en flow</span><span class="sxs-lookup"><span data-stu-id="49d6f-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


