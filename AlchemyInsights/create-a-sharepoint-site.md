---
title: Een SharePoint-site maken
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806934"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4520e-102">Een SharePoint-site maken</span><span class="sxs-lookup"><span data-stu-id="4520e-102">Create a SharePoint site</span></span>

<span data-ttu-id="4520e-103">Sites maken of beheren op basis van [actieve sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in het SharePoint-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="4520e-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="4520e-104">Zie [sites beheren in het nieuwe SharePoint-Beheercentrum](https://docs.microsoft.com/sharepoint/manage-site-creation)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4520e-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="4520e-105">Hoe</span><span class="sxs-lookup"><span data-stu-id="4520e-105">Tips:</span></span>

- <span data-ttu-id="4520e-106">U **kunt** geen site maken met dezelfde URL van een bestaande site.</span><span class="sxs-lookup"><span data-stu-id="4520e-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4520e-107">Als u een site hebt verwijderd en de URL opnieuw wilt gebruiken, is de verwijderde site mogelijk aanwezig onder [Verwijderde sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="4520e-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="4520e-108">De site moet permanent worden verwijderd om de URL opnieuw te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="4520e-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="4520e-109">Als u een site geheel wilt verwijderen met PowerShell, raadpleegt u het voorbeeld van de cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="4520e-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="4520e-110">Sommige gebruikers kunnen geen site maken.</span><span class="sxs-lookup"><span data-stu-id="4520e-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="4520e-111">[Zie sites maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4520e-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="4520e-112">Het is mogelijk dat de site blijft hangen bij het **maken** van een langer dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="4520e-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4520e-113">Als het probleem zich nog steeds voordoet, kunt u een ondersteuningsticket registreren als u meer dan 24 uur hebt verstreken sinds u het eerst hebt gezien.</span><span class="sxs-lookup"><span data-stu-id="4520e-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4520e-114">In veel gevallen werken we al met een oplossing.</span><span class="sxs-lookup"><span data-stu-id="4520e-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4520e-115">Geef ons minstens 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="4520e-115">Please give us at least 24 hours to complete a solution.</span></span>
