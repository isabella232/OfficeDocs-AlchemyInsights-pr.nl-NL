---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694451"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="9ddb1-102">Openen met Explorer werkt niet</span><span class="sxs-lookup"><span data-stu-id="9ddb1-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="9ddb1-103">Als **openen met Verkenner** of **weergave in de Verkenner** niet werkt, controleert u of de WebClient-service is ingesteld om te worden **uitgevoerd** door de onderstaande stappen te volgen.</span><span class="sxs-lookup"><span data-stu-id="9ddb1-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="9ddb1-104">Het kan enige tijd duren voordat u een SharePoint-of OneDrive-bibliotheek opent wanneer de service niet actief is.</span><span class="sxs-lookup"><span data-stu-id="9ddb1-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="9ddb1-105">Typ in het vak Windows Search de tekst run, selecteer de bureaublad-app uitvoeren, typ services. msc en selecteer vervolgens **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9ddb1-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="9ddb1-106">Schuif omlaag naar de WebClient service en kijk in de kolom **status** .</span><span class="sxs-lookup"><span data-stu-id="9ddb1-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="9ddb1-107">Als de status van de client service niet **actief**is, dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="9ddb1-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9ddb1-108">Schakel de service, indien nodig, in en selecteer **handmatig** of **automatisch** in het vak **Opstarttype** .</span><span class="sxs-lookup"><span data-stu-id="9ddb1-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9ddb1-109">Zie [openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor informatie over het oplossen van problemen met openen in de Verkenner.</span><span class="sxs-lookup"><span data-stu-id="9ddb1-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9ddb1-110">Ontdek de synchronisatie als een beter alternatief: [SharePoint-bestanden synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9ddb1-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

