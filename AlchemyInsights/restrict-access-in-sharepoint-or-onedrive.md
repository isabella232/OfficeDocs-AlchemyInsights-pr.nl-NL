---
title: Toegang in SharePoint of OneDrive beperken
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715879"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d3a90-102">Toegang in SharePoint of OneDrive beperken</span><span class="sxs-lookup"><span data-stu-id="d3a90-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d3a90-103">In SharePoint en OneDrive beperkt u de toegang tot items zoals bestanden, mappen en lijsten door alleen toegang te verlenen aan groepen of personen die u toegang wilt hebben.</span><span class="sxs-lookup"><span data-stu-id="d3a90-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="d3a90-104">Standaard worden machtigingen in SharePoint overgenomen van hoger in de hiërarchie.</span><span class="sxs-lookup"><span data-stu-id="d3a90-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="d3a90-105">Een bestand erft dus zijn machtigingen van de map, die de machtigingen ervan overneemt van de bibliotheek, die de machtigingen van de site erft.</span><span class="sxs-lookup"><span data-stu-id="d3a90-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="d3a90-106">U delen op een hoger niveau (bijvoorbeeld door het delen van een hele site) en vervolgens breken erfenis als u niet wilt dat alle items op de site te delen.</span><span class="sxs-lookup"><span data-stu-id="d3a90-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="d3a90-107">We raden dit echter niet aan omdat het onderhouden van de machtigingen in de toekomst complexer en verwarrender wordt.</span><span class="sxs-lookup"><span data-stu-id="d3a90-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="d3a90-108">Dit is wat je in plaats daarvan zou kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="d3a90-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="d3a90-109">Als u bijvoorbeeld alle inhoud van een map wilt delen, behalve één bestand erin, verplaatst u dat bestand naar een nieuwe locatie die niet wordt gedeeld.</span><span class="sxs-lookup"><span data-stu-id="d3a90-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="d3a90-110">Als u twee submappen in een map hebt en u één submap wilt delen met de groepen A en B en alleen groep A toegang wilt geven tot de tweede submap, deelt u de bovenliggende map met groep A en voegt u groep B toe aan de eerste submap.</span><span class="sxs-lookup"><span data-stu-id="d3a90-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="d3a90-111">Het delen van een bestand of map stoppen</span><span class="sxs-lookup"><span data-stu-id="d3a90-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

