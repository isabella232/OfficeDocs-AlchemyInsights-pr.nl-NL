---
title: Beperk de toegang in de SharePoint- of OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383866"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b8017-102">Beperk de toegang in de SharePoint- of OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8017-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b8017-103">In SharePoint en OneDrive beperken u toegang tot items zoals bestanden, mappen en lijsten door toegang alleen voor groepen of personen die u toegang wilt verlenen.</span><span class="sxs-lookup"><span data-stu-id="b8017-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b8017-104">Standaard worden machtigingen in SharePoint worden overgenomen van hogere omhoog in de hiërarchie.</span><span class="sxs-lookup"><span data-stu-id="b8017-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b8017-105">Een bestand wordt dus de machtigingen overneemt van de map de machtigingen worden overgenomen uit de bibliotheek waarvan de machtigingen worden overgenomen van de site.</span><span class="sxs-lookup"><span data-stu-id="b8017-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b8017-106">U kunt delen op een hoger niveau (bijvoorbeeld door het delen van een hele site) en vervolgens overnemen als u niet wilt dat de artikelen op de site delen.</span><span class="sxs-lookup"><span data-stu-id="b8017-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b8017-107">Echter niet aangeraden dit omdat het onderhoud van de machtigingen meer complex en verwarrend zijn in de toekomst maakt.</span><span class="sxs-lookup"><span data-stu-id="b8017-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b8017-108">Dit is wat u in plaats daarvan kan doen:</span><span class="sxs-lookup"><span data-stu-id="b8017-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b8017-109">Als u bijvoorbeeld de inhoud van een map, met uitzondering van één bestand delen wilt, verplaatst u dat bestand naar een nieuwe locatie die niet wordt gedeeld.</span><span class="sxs-lookup"><span data-stu-id="b8017-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b8017-110">Als u twee submappen in een map hebt en u wilt een submap delen met groepen A en B en alleen groep A toegang tot het tweede mapniveau, delen van de bovenliggende map bij groep A en B-groep toevoegen aan de eerste submap.</span><span class="sxs-lookup"><span data-stu-id="b8017-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b8017-111">Delen van een bestand of map beëindigen</span><span class="sxs-lookup"><span data-stu-id="b8017-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

