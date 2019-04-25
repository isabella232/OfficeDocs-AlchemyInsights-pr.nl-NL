---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419864"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="49a32-102">Openen met Explorer werkt niet</span><span class="sxs-lookup"><span data-stu-id="49a32-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="49a32-103">Als **openen met Explorer** of **weergave in File Explorer** werkt niet controleren of dat de WebClient-service is ingesteld op **wordt uitgevoerd** door de onderstaande stappen te volgen.</span><span class="sxs-lookup"><span data-stu-id="49a32-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="49a32-104">Het duurt zo lang voor het openen van een documentbibliotheek van SharePoint of OneDrive als de service niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="49a32-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="49a32-105">Selecteer in het zoekvak van Windows, type uitvoert, de desktop app Run, type services.msc en klik vervolgens op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="49a32-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="49a32-106">Blader naar de WebClient-service en de kolom **Status** .</span><span class="sxs-lookup"><span data-stu-id="49a32-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="49a32-107">Als de status van de WebClient-service niet **wordt uitgevoerd**, dubbelklikt u op de service, klikt u op **Start**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="49a32-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="49a32-108">Schakel de service, als deze nodig zijn, **handmatig** of **automatisch** selecteren in het vak **Opstarttype** .</span><span class="sxs-lookup"><span data-stu-id="49a32-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="49a32-109">Zie [openen in Explorer](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in File Explorer te openen.</span><span class="sxs-lookup"><span data-stu-id="49a32-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="49a32-110">Ontdek synchroniseren als een beter alternatief: [Sync SharePoint-bestanden met de nieuwe OneDrive synchronisatie-client](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="49a32-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

