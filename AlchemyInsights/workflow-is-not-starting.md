---
title: Werkstroom start niet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403738"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="225f8-102">Werkstroom start niet</span><span class="sxs-lookup"><span data-stu-id="225f8-102">Workflow is not starting</span></span>

- <span data-ttu-id="225f8-103">SharePoint 2010- en SharePoint 2013-werkstromen beginnen niet.</span><span class="sxs-lookup"><span data-stu-id="225f8-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="225f8-104">Als uw werkstroom niet wordt begonnen, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers mogelijk met af en toe vertragingen met de voortgang van de werkstroom te maken kunnen krijgen.</span><span class="sxs-lookup"><span data-stu-id="225f8-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="225f8-105">Controleer het [dashboard Service health om](https://admin.microsoft.com/AdminPortal/Home/servicehealth) te zien of uw organisatie wordt beïnvloed.</span><span class="sxs-lookup"><span data-stu-id="225f8-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="225f8-106">Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst hebt gezien, moet u een ondersteuningsticket aanmelden.</span><span class="sxs-lookup"><span data-stu-id="225f8-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="225f8-107">In veel gevallen werken we al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="225f8-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="225f8-108">Geef ons ten minste 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="225f8-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="225f8-109">SharePoint 2010-werkstromen zijn vertraagd bij de start.</span><span class="sxs-lookup"><span data-stu-id="225f8-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="225f8-110">Dit gebeurt als de werkstroom wordt geactiveerd in grote batches.</span><span class="sxs-lookup"><span data-stu-id="225f8-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="225f8-111">(bijvoorbeeld wanneer er meerdere items tegelijk worden toegevoegd).</span><span class="sxs-lookup"><span data-stu-id="225f8-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="225f8-112">Werkstromen zijn niet ontworpen om realtime uit te voeren, dus een vertraging is ontwerpgedrag.</span><span class="sxs-lookup"><span data-stu-id="225f8-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="225f8-113">Als de werkstroom complex is Extensible Object Markup Language (XMOL), kan de compilatie traag zijn.</span><span class="sxs-lookup"><span data-stu-id="225f8-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="225f8-114">Controleer [dit](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="225f8-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="225f8-115">U moet de werkstroom vereenvoudigen of deze opnieuw ontwerpen met behulp van het type Microsoft SharePoint 2013-werkstroomplatform.</span><span class="sxs-lookup"><span data-stu-id="225f8-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="225f8-116">Als de werkstroomgeschiedenis groot is geworden, kunt u de items verwijderen of een nieuwe geschiedenislijst maken.</span><span class="sxs-lookup"><span data-stu-id="225f8-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="225f8-117">Meer informatie: [Werkstroomgeschiedenis verwijderen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="225f8-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="225f8-118">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="225f8-118">Related topics</span></span>
<span data-ttu-id="225f8-119">Wilt u Microsoft Flow proberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="225f8-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="225f8-120">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="225f8-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="225f8-121">SharePoint en Flow</span><span class="sxs-lookup"><span data-stu-id="225f8-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
