---
title: Een SharePoint-site maken
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802961"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="86192-102">Een SharePoint-site maken</span><span class="sxs-lookup"><span data-stu-id="86192-102">Create a SharePoint site</span></span>

<span data-ttu-id="86192-103">Hier ziet u de volgende onderwerpen voor informatie over het maken van SharePoint-site:</span><span class="sxs-lookup"><span data-stu-id="86192-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="86192-104">[Sites beheren in de nieuwe SharePoint-admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): informatie over het maken van opties, waaronder het maken van een klassieke site of een site voor teams waarin een Office 365-groep niet.</span><span class="sxs-lookup"><span data-stu-id="86192-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="86192-105">[Een team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): informatie over het maken van een teamsite.</span><span class="sxs-lookup"><span data-stu-id="86192-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="86192-106">[Een communicatie-site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): informatie over het maken van een communicatie-site.</span><span class="sxs-lookup"><span data-stu-id="86192-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="86192-107">[Sites beheren in de nieuwe SharePoint-admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): informatie over het maken van een klassieke site of een site met een Office 365-groep niet.</span><span class="sxs-lookup"><span data-stu-id="86192-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tips]
> - <span data-ttu-id="86192-109">U kunt een site maken met de URL van een bestaande site.</span><span class="sxs-lookup"><span data-stu-id="86192-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="86192-110">Als u een site verwijderd en willen de URL opnieuw te gebruiken, is het mogelijk dat verwijderde site bestaat nog steeds onder **sites verwijderd**.</span><span class="sxs-lookup"><span data-stu-id="86192-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="86192-111">Verwijderd voor het beheren van websites Zie, [een Site verwijderen](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="86192-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="86192-112">Als u wilt volledig verwijderen van een site met Powershell, Zie het voorbeeld van de cmdlet [Verwijderen SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="86192-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="86192-113">Sommige gebruikers misschien niet mogelijk om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="86192-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="86192-114">Zie [beheren sites maken in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="86192-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="86192-115">Het is mogelijk dat de site wordt weergegeven op **maken** langer dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="86192-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="86192-116">Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst zag, meld u een support ticket.</span><span class="sxs-lookup"><span data-stu-id="86192-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="86192-117">In veel gevallen hebben werkt we aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="86192-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="86192-118">Geef ons ten minste 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="86192-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="86192-119">Als u nodig hebt voor het maken van een nieuwe teamsite opnemen die een Office 365-groep niet</span><span class="sxs-lookup"><span data-stu-id="86192-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


