---
title: Werkstroom wordt niet gestart
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794762"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="490e0-102">Werkstroom wordt niet gestart</span><span class="sxs-lookup"><span data-stu-id="490e0-102">Workflow is not starting</span></span>

- <span data-ttu-id="490e0-103">Werkstromen van SharePoint 2010 en SharePoint 2013 worden niet gestart.</span><span class="sxs-lookup"><span data-stu-id="490e0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="490e0-104">Als de werkstroom niet kan worden gestart, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers de werkstroom af en toe kunnen zien.</span><span class="sxs-lookup"><span data-stu-id="490e0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="490e0-105">Controleer het [Dashboard service status](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie van invloed is.</span><span class="sxs-lookup"><span data-stu-id="490e0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="490e0-106">Als het probleem zich nog steeds voordoet, kunt u een ondersteuningsticket registreren als u meer dan 24 uur hebt verstreken sinds u het eerst hebt gezien.</span><span class="sxs-lookup"><span data-stu-id="490e0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="490e0-107">In veel gevallen werken we al met een oplossing.</span><span class="sxs-lookup"><span data-stu-id="490e0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="490e0-108">Geef ons minstens 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="490e0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="490e0-109">SharePoint 2010-werkstromen vertraagd bij start.</span><span class="sxs-lookup"><span data-stu-id="490e0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="490e0-110">Dit gebeurt als de werkstroom wordt geactiveerd in grote batches.</span><span class="sxs-lookup"><span data-stu-id="490e0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="490e0-111">(bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).</span><span class="sxs-lookup"><span data-stu-id="490e0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="490e0-112">Werkstromen zijn niet ontworpen voor het uitvoeren van realtime en daarom is een vertraging inherent aan het ontwerp gedrag.</span><span class="sxs-lookup"><span data-stu-id="490e0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="490e0-113">Als de werkstroom complexe Extensible object Markup Language (XMOL) is, kan de compilatie traag worden.</span><span class="sxs-lookup"><span data-stu-id="490e0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="490e0-114">Raadpleeg [Dit](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="490e0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="490e0-115">U dient de werkstroom te vereenvoudigen of opnieuw te ontwerpen met het type Microsoft SharePoint 2013-werkstroom platform.</span><span class="sxs-lookup"><span data-stu-id="490e0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="490e0-116">Als uw werkstroomgeschiedenis groot is geworden, kunt u de items verwijderen of een nieuwe geschiedenislijst maken.</span><span class="sxs-lookup"><span data-stu-id="490e0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="490e0-117">Meer informatie: [werkstroomgeschiedenis wissen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="490e0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="490e0-118">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="490e0-118">Related topics</span></span>
<span data-ttu-id="490e0-119">Wilt u Microsoft flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="490e0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="490e0-120">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="490e0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="490e0-121">SharePoint en flow</span><span class="sxs-lookup"><span data-stu-id="490e0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


