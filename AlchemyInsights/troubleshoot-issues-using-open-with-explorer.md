---
title: Oplossen van problemen met de functie openen met Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390602"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2a87a-102">Oplossen van problemen met het openen met Explorer</span><span class="sxs-lookup"><span data-stu-id="2a87a-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2a87a-103">Veelvoorkomende problemen bij het openen van een documentbibliotheek in SharePoint of OneDrive met de opdracht **openen met Explorer** oplossen:</span><span class="sxs-lookup"><span data-stu-id="2a87a-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2a87a-104">Gebruik Internet Explorer 10 of Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="2a87a-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2a87a-105">**Openen met Explorer** is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="2a87a-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a87a-106">**Openen met Explorer** is in alle browsers behalve Internet Explorer uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="2a87a-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a87a-107">**Openen met Explorer** is niet beschikbaar in de moderne ervaring voor SharePoint-bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="2a87a-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2a87a-108">**Weergave in File Explorer** te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="2a87a-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2a87a-109">Selecteer **weergave-opties** \> **weergave in File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="2a87a-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2a87a-110">Weergave in File Explorer is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="2a87a-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a87a-111">**Weergave in File Explorer** in alleen beschikbaar in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a87a-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a87a-112">Controleer of dat de WebClient-service wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="2a87a-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2a87a-113">Selecteer de desktop app uitvoeren in het zoekvak van Windows, type uitvoeren, typ services.msc en druk op Enter.</span><span class="sxs-lookup"><span data-stu-id="2a87a-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2a87a-114">Schuif naar de WebClient-service en controleer of dat de kolom **Status** wordt 'Uitvoeren'.</span><span class="sxs-lookup"><span data-stu-id="2a87a-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2a87a-115">Als dat niet het geval is, dubbelklikt u op de service, klikt u op **Start**en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="2a87a-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2a87a-116">(Mogelijk moet u eerst de service inschakelen door **handmatig** of **automatisch** selecteren in het vak **Opstarttype** .)</span><span class="sxs-lookup"><span data-stu-id="2a87a-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2a87a-117">Een bibliotheek openen in Verkenner is handig als u wilt kopiëren of verplaatsen van meerdere bestanden en mappen na, maar als u regelmatig werkt in de bibliotheek wilt maken, wordt aangeraden deze te synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="2a87a-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2a87a-118">Zie [openen in Explorer](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in File Explorer te openen.</span><span class="sxs-lookup"><span data-stu-id="2a87a-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2a87a-119">Zie voor informatie over het instellen van sync, [Sync SharePoint-bestanden met de nieuwe OneDrive synchronisatie-client](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2a87a-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2a87a-120">Zie het artikel [het gebruik van de opdracht ' openen met Explorer ' oplossen van problemen in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2a87a-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

