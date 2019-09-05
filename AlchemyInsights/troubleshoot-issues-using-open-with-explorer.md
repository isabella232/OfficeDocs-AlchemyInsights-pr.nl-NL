---
title: Problemen met openen met Verkenner oplossen
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742728"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="1546d-102">Problemen met openen met Verkenner oplossen</span><span class="sxs-lookup"><span data-stu-id="1546d-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="1546d-103">Veelvoorkomende problemen oplossen met het openen van een documentbibliotheek in SharePoint of OneDrive met de opdracht **openen met Verkenner** :</span><span class="sxs-lookup"><span data-stu-id="1546d-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="1546d-104">Internet Explorer 10 of Internet Explorer 11 gebruiken.</span><span class="sxs-lookup"><span data-stu-id="1546d-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="1546d-105">**Openen met Explorer** is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="1546d-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1546d-106">**Openen met Verkenner** is uitgeschakeld in alle browsers behalve Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="1546d-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="1546d-107">**Openen met Explorer** is niet beschikbaar in de moderne ervaring voorsharepoint-bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="1546d-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="1546d-108">Gebruik **in plaats daarvan weergave in Verkenner** .</span><span class="sxs-lookup"><span data-stu-id="1546d-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="1546d-109">Selecteer weergave **Opties** \> **weergeven in Verkenner**.</span><span class="sxs-lookup"><span data-stu-id="1546d-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="1546d-110">View in File Explorer is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="1546d-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1546d-111">**Weergeven in bestandsverkenner** in alleen beschikbaar in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="1546d-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="1546d-112">Zorg ervoor dat de WebClient-service wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="1546d-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="1546d-113">Typ in het zoekvak van Windows uitvoeren, selecteer de desktop-app uitvoeren, typ services. msc en druk op ENTER.</span><span class="sxs-lookup"><span data-stu-id="1546d-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="1546d-114">Scrol omlaag naar de WebClient-service en zorg ervoor dat in de kolom **status** ' actief ' wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="1546d-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="1546d-115">Als dit niet het, dubbelklikt u op de service, klikt u op **Start**, en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="1546d-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="1546d-116">(Mogelijk moet u de service eerst inschakelen door **handmatig** of **automatisch** te selecteren in het vak **Opstarttype** .)</span><span class="sxs-lookup"><span data-stu-id="1546d-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1546d-117">Het openen van een bibliotheek in Verkenner is handig als u meerdere bestanden en mappen eenmaal moet kopiëren of verplaatsen, maar als u regelmatig in de bibliotheek wilt werken, raden we u aan deze te synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="1546d-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="1546d-118">Zie [openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)om problemen met het openen van bestanden in Verkenner op te lossen.</span><span class="sxs-lookup"><span data-stu-id="1546d-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="1546d-119">Zie voor meer informatie over [het instellen van Synchronisatieshare Point-bestanden synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="1546d-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="1546d-120">Raadpleeg het artikel [het gebruik van de opdracht ' openen met Explorer ' voor het oplossen van problemen in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1546d-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

