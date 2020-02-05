---
title: Een SharePoint-site maken
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770850"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="39876-102">Een SharePoint-site maken</span><span class="sxs-lookup"><span data-stu-id="39876-102">Create a SharePoint site</span></span>

<span data-ttu-id="39876-103">Sites maken of beheren vanuit [actieve sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in het SharePoint-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="39876-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="39876-104">Zie [Sites beheren in het nieuwe SharePoint-beheercentrum](https://docs.microsoft.com/sharepoint/manage-site-creation)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="39876-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="39876-105">Tips:</span><span class="sxs-lookup"><span data-stu-id="39876-105">Tips:</span></span>

- <span data-ttu-id="39876-106">U **kunt geen** site maken met dezelfde URL van een bestaande site.</span><span class="sxs-lookup"><span data-stu-id="39876-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="39876-107">Als u een site hebt verwijderd en de URL opnieuw wilt gebruiken, is het mogelijk dat de verwijderde site nog steeds bestaat onder [Verwijderde sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="39876-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="39876-108">De site moet permanent worden verwijderd om de URL opnieuw te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="39876-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="39876-109">Zie het voorbeeld [Verwijderen-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet om een site volledig te verwijderen met Powershell.</span><span class="sxs-lookup"><span data-stu-id="39876-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="39876-110">Sommige gebruikers kunnen mogelijk geen site maken.</span><span class="sxs-lookup"><span data-stu-id="39876-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="39876-111">[Zie Sitemaken beheren in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="39876-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="39876-112">Het is mogelijk dat de site langer vast lijkt te zitten bij **Het maken** van langer dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="39876-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="39876-113">Als er meer dan 24 uur zijn verstreken sinds je dit probleem voor het eerst hebt gezien, log dan een ondersteuningsticket in.</span><span class="sxs-lookup"><span data-stu-id="39876-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="39876-114">In veel gevallen werken we al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="39876-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="39876-115">Geef ons minstens 24 uur de tijd om een oplossing te vinden.</span><span class="sxs-lookup"><span data-stu-id="39876-115">Please give us at least 24 hours to complete a solution.</span></span>
