---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283622"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="a2dc4-102">Openen met Explorer werkt niet</span><span class="sxs-lookup"><span data-stu-id="a2dc4-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="a2dc4-p101">Als **openen met Explorer** of **weergave in File Explorer** werkt niet controleren of dat de WebClient-service is ingesteld op **wordt uitgevoerd** door de onderstaande stappen te volgen. Het duurt zo lang voor het openen van een documentbibliotheek van SharePoint of OneDrive als de service niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a2dc4-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="a2dc4-105">Selecteer in het zoekvak van Windows, type uitvoert, de desktop app Run, type services.msc en klik vervolgens op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a2dc4-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="a2dc4-p102">Blader naar de WebClient-service en de kolom **Status** . Als de status van de WebClient-service niet **wordt uitgevoerd**, dubbelklikt u op de service, klikt u op **Start**en klik vervolgens op **OK**. Schakel de service, als deze nodig zijn, **handmatig** of **automatisch** selecteren in het vak **Opstarttype** .</span><span class="sxs-lookup"><span data-stu-id="a2dc4-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a2dc4-p103">Zie [openen in Explorer](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in File Explorer te openen. Ontdek synchroniseren als een beter alternatief: [Sync SharePoint-bestanden met de nieuwe OneDrive synchronisatie-client](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a2dc4-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

