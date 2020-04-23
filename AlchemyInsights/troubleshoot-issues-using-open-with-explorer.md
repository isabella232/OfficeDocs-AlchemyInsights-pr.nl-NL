---
title: Problemen oplossen met Openen met Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759687"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="ad794-102">Problemen met Openen met Explorer oplossen</span><span class="sxs-lookup"><span data-stu-id="ad794-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="ad794-103">Veelvoorkomende problemen oplossen bij het openen van een documentbibliotheek in SharePoint of OneDrive met de opdracht **Openen met Explorer:**</span><span class="sxs-lookup"><span data-stu-id="ad794-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="ad794-104">Gebruik Internet Explorer 10 of Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="ad794-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="ad794-105">**Open with Explorer** is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="ad794-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="ad794-106">**Openen met Explorer** is uitgeschakeld in alle browsers behalve In Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad794-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="ad794-107">**Openen met Explorer** is niet beschikbaar in de moderne ervaring voor SharePoint-bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="ad794-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="ad794-108">Gebruik weergave in plaats daarvan **in Verkenner.**</span><span class="sxs-lookup"><span data-stu-id="ad794-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="ad794-109">Selecteer **Weergaveopties** \> **weergeven in Verkenner**.</span><span class="sxs-lookup"><span data-stu-id="ad794-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="ad794-110">Weergave in Verkenner is niet compatibel met Microsoft Edge, Google Chrome, Firefox en anderen.</span><span class="sxs-lookup"><span data-stu-id="ad794-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="ad794-111">**Bekijk in Verkenner** alleen beschikbaar in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad794-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="ad794-112">Controleer of de WebClient-service wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="ad794-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="ad794-113">Typ in het zoekvak Van Windows uitvoeren, selecteer de bureaublad-app uitvoeren, typ services.msc en druk op Enter.</span><span class="sxs-lookup"><span data-stu-id="ad794-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="ad794-114">Schuif omlaag naar de WebClient-service en controleer of in de kolom **Status** 'Actief' wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="ad794-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="ad794-115">Als dit niet het zo is, dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="ad794-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="ad794-116">(Mogelijk moet u de service eerst inschakelen door **Handmatig** of **automatisch** te selecteren in het vak **Opstarttype.)**</span><span class="sxs-lookup"><span data-stu-id="ad794-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ad794-117">Het openen van een bibliotheek in Verkenner is handig als u meerdere bestanden en mappen één keer wilt kopiëren of verplaatsen, maar als u regelmatig in de bibliotheek wilt werken, raden we u aan deze te synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="ad794-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="ad794-118">Zie [Openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in Verkenner.</span><span class="sxs-lookup"><span data-stu-id="ad794-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="ad794-119">Zie [SharePoint-bestanden synchroniseren met de nieuwe Synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666)van OneDrive voor meer informatie over het instellen van synchronisatie.</span><span class="sxs-lookup"><span data-stu-id="ad794-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="ad794-120">Zie het artikel [Hoe u de opdracht Openen met Explorer gebruiken om problemen in SharePoint Online op te lossen](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ad794-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

