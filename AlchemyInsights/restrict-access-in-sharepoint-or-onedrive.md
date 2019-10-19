---
title: Toegang beperken in SharePoint of OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551446"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="62c37-102">Toegang beperken in SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="62c37-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="62c37-103">In SharePoint en OneDrive beperkt u de toegang tot items zoals bestanden, mappen en lijsten door alleen toegang te verlenen aan groepen of personen die u toegang wilt geven.</span><span class="sxs-lookup"><span data-stu-id="62c37-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="62c37-104">Machtigingen in SharePoint worden standaard overgenomen van hoger in de hiërarchie.</span><span class="sxs-lookup"><span data-stu-id="62c37-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="62c37-105">Een bestand neemt dus zijn machtigingen over van de map, die zijn machtigingen overneemt van de bibliotheek, die zijn machtigingen overneemt van de site.</span><span class="sxs-lookup"><span data-stu-id="62c37-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="62c37-106">U op een hoger niveau delen (bijvoorbeeld door een hele site te delen) en vervolgens overname verbreken als u niet alle items op de site wilt delen.</span><span class="sxs-lookup"><span data-stu-id="62c37-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="62c37-107">We raden dit echter niet aan omdat het het onderhouden van de machtigingen in de toekomst complexer en verwarrend maakt.</span><span class="sxs-lookup"><span data-stu-id="62c37-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="62c37-108">Dit is wat je in plaats daarvan zou kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="62c37-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="62c37-109">Als u bijvoorbeeld alle inhoud van een map wilt delen, behalve één bestand erin, verplaatst u dat bestand naar een nieuwe locatie die niet wordt gedeeld.</span><span class="sxs-lookup"><span data-stu-id="62c37-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="62c37-110">Als u twee submappen in een map hebt en u een submap met groepen A en B wilt delen en alleen groepstoegang tot de tweede submap wilt toestaan, deelt u de bovenliggende map met groep A en voegt u groep B toe aan de eerste submap.</span><span class="sxs-lookup"><span data-stu-id="62c37-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="62c37-111">Het delen van een bestand of map beëindigen</span><span class="sxs-lookup"><span data-stu-id="62c37-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

