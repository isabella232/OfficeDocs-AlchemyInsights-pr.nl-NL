---
title: Toegang beperken in SharePoint of OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720677"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="91d44-102">Toegang beperken in SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="91d44-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="91d44-103">In SharePoint en OneDrive beperkt u de toegang tot items zoals bestanden, mappen en lijsten door alleen toegang te verlenen aan groepen of individuele gebruikers waartoe u toegang wilt hebben.</span><span class="sxs-lookup"><span data-stu-id="91d44-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="91d44-104">Machtigingen in SharePoint worden standaard overgenomen van hoger in de hiërarchie.</span><span class="sxs-lookup"><span data-stu-id="91d44-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="91d44-105">Zodat een bestand de machtigingen van de map overneemt, welke machtigingen van de bibliotheek overnemen en de machtigingen van de site overnemen.</span><span class="sxs-lookup"><span data-stu-id="91d44-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="91d44-106">U kunt op een hoger niveau delen (bijvoorbeeld door een hele site te delen) en vervolgens de overname van machtigingen stoppen als u niet alle items op de site wilt delen.</span><span class="sxs-lookup"><span data-stu-id="91d44-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="91d44-107">We raden u echter niet aan dat u dit kunt doen omdat u de machtigingen in de toekomst eenvoudiger en verwarrend houdt.</span><span class="sxs-lookup"><span data-stu-id="91d44-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="91d44-108">U kunt in plaats hiervan het volgende doen:</span><span class="sxs-lookup"><span data-stu-id="91d44-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="91d44-109">Als u bijvoorbeeld de inhoud van een map met uitzondering van een bestand wilt delen, verplaatst u het bestand naar een andere locatie die niet wordt gedeeld.</span><span class="sxs-lookup"><span data-stu-id="91d44-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="91d44-110">Als u twee submappen in een map hebt en u wilt één submap met de groepen A en B delen en alleen groepen toegang verlenen tot de tweede submap, deelt u de bovenliggende map met groep A en voegt u groep B toe aan de eerste submap.</span><span class="sxs-lookup"><span data-stu-id="91d44-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="91d44-111">Het delen van een bestand of map stoppen </span><span class="sxs-lookup"><span data-stu-id="91d44-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

