---
title: Verwijder permanent een site in SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955129"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="4d777-102">Verwijder permanent een site in SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d777-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="4d777-103">Om een URL van een verwijderde site opnieuw te gebruiken (om een site opnieuw te maken) of om een site permanent te verwijderen omdat deze niet langer in gebruik is, kunt u \*\* Permanent verwijderen \*\* gebruiken in het nieuwe SharePoint Admin Center.</span><span class="sxs-lookup"><span data-stu-id="4d777-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="4d777-104">Ga naar de [ pagina met verwijderde sites van het nieuwe SharePoint-beheercentrum ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) en log in met een account dat beheerdersrechten heeft voor uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="4d777-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="4d777-105">Selecteer in de linkerkolom een site.</span><span class="sxs-lookup"><span data-stu-id="4d777-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="4d777-106">Klik op \*\* Permanent verwijderen \*\*.</span><span class="sxs-lookup"><span data-stu-id="4d777-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="4d777-107">\*\* Opmerking \*\*: Groepsgebonden sites kunnen niet permanent worden verwijderd uit het nieuwe SharePoint Admin Center.</span><span class="sxs-lookup"><span data-stu-id="4d777-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="4d777-108">In plaats daarvan moet [ Remove-SPODeletedSite ](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4d777-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="4d777-109">Zie [ Een site definitief verwijderen ](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4d777-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
