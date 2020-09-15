---
title: Problemen oplossen met openen met Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659053"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="79d49-102">Problemen oplossen met openen met Explorer</span><span class="sxs-lookup"><span data-stu-id="79d49-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="79d49-103">Veelvoorkomende problemen met het openen van een documentbibliotheek in SharePoint of OneDrive oplossen met de opdracht **openen met Explorer** :</span><span class="sxs-lookup"><span data-stu-id="79d49-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="79d49-104">Internet Explorer 10 of Internet Explorer 11 gebruiken.</span><span class="sxs-lookup"><span data-stu-id="79d49-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="79d49-105">**Openen met Explorer** is niet compatibel met Microsoft Edge, Google Chrome, Firefox en andere.</span><span class="sxs-lookup"><span data-stu-id="79d49-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="79d49-106">**Openen met Explorer** is uitgeschakeld in alle browsers, met uitzondering van Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="79d49-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="79d49-107">**Openen met Explorer** is niet beschikbaar in de moderne ervaring voor SharePoint-bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="79d49-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="79d49-108">Gebruik in plaats hiervan **weergave in Verkenner** .</span><span class="sxs-lookup"><span data-stu-id="79d49-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="79d49-109">Selecteer weergave **Opties** \> **weergeven in Verkenner**.</span><span class="sxs-lookup"><span data-stu-id="79d49-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="79d49-110">Weergeven in bestandenverkenner is niet compatibel met Microsoft Edge, Google Chrome, Firefox en andere.</span><span class="sxs-lookup"><span data-stu-id="79d49-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="79d49-111">**Weergeven in de Verkenner** in alleen beschikbaar in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="79d49-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="79d49-112">Zorg ervoor dat de client service wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="79d49-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="79d49-113">Typ in het vak Windows Search de tekst run, selecteer de bureaublad-app uitvoeren, typ services. msc en druk op ENTER.</span><span class="sxs-lookup"><span data-stu-id="79d49-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="79d49-114">Schuif omlaag naar de WebClient service en zorg ervoor dat in de kolom **status** de waarde ' uitvoeren ' wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="79d49-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="79d49-115">Als dit niet het geval is, dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="79d49-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="79d49-116">(Mogelijk moet u eerst de service inschakelen door **handmatig** of **automatisch** in het vak **Opstarttype** te selecteren.)</span><span class="sxs-lookup"><span data-stu-id="79d49-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="79d49-117">Het openen van een bibliotheek in Verkenner is handig als u meerdere bestanden en mappen wilt kopiëren of verplaatsen, maar als u regelmatig wilt werken in de bibliotheek, is het raadzaam om deze te synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="79d49-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="79d49-118">Zie [openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor informatie over het oplossen van problemen met openen in de Verkenner.</span><span class="sxs-lookup"><span data-stu-id="79d49-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="79d49-119">Voor informatie over het instellen van synchronisatie raadpleegt u [SharePoint-bestanden synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="79d49-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="79d49-120">Zie het artikel [hoe u met de opdracht ' openen met Explorer ' problemen oplost in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="79d49-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

