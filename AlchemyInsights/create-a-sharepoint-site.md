---
title: Een SharePoint-site maken
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738192"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="10b45-102">Een SharePoint-site maken</span><span class="sxs-lookup"><span data-stu-id="10b45-102">Create a SharePoint site</span></span>

<span data-ttu-id="10b45-103">U het volgende zien voor informatie over het maken van SharePoint-sites:</span><span class="sxs-lookup"><span data-stu-id="10b45-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="10b45-104">[Sites beheren in het nieuwe SharePoint-Beheercentrum](https://docs.microsoft.com/sharepoint/manage-site-creation): meer informatie over opties voor site creatie, waaronder het maken van een klassieke site of een teams-site die geen Office 365-groep bevat.</span><span class="sxs-lookup"><span data-stu-id="10b45-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="10b45-105">[Een team site maken in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): meer informatie over het maken van een team site.</span><span class="sxs-lookup"><span data-stu-id="10b45-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="10b45-106">[Een communicatiesite maken in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): meer informatie over het maken van een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="10b45-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="10b45-107">[Sites beheren in het nieuwe SharePoint-Beheercentrum](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): meer informatie over het maken van een klassieke site of een team site die geen Office 365-groep bevat.</span><span class="sxs-lookup"><span data-stu-id="10b45-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="10b45-108">[! Tips</span><span class="sxs-lookup"><span data-stu-id="10b45-108">[!Tips]</span></span>
> - <span data-ttu-id="10b45-109">U geen site maken met dezelfde URL van een bestaande site.</span><span class="sxs-lookup"><span data-stu-id="10b45-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="10b45-110">Als u een site hebt verwijderd en de URL opnieuw wilt gebruiken, is het mogelijk dat de verwijderde site nog steeds bestaat onder **Verwijderde sites**.</span><span class="sxs-lookup"><span data-stu-id="10b45-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="10b45-111">Als je verwijderde sites wilt beheren, zie je [een site verwijderen](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="10b45-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="10b45-112">Als u een site met PowerShell volledig wilt verwijderen, raadpleegt u het voorbeeld van de cmdlet [Remove SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="10b45-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="10b45-113">Het is mogelijk dat sommige gebruikers geen site kunnen maken.</span><span class="sxs-lookup"><span data-stu-id="10b45-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="10b45-114">Zie [site maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="10b45-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="10b45-115">Het is mogelijk dat de site lijkt te zijn vastgelopen bij **het maken van** langer dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="10b45-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="10b45-116">Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst zag, logt u een ondersteuningsticket in.</span><span class="sxs-lookup"><span data-stu-id="10b45-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="10b45-117">In veel gevallen werken we nu al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="10b45-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="10b45-118">Gelieve ons ten minste 24 uur te geven om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="10b45-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="10b45-119">Als u een nieuwe team site moet maken die geen Office 365-groep bevat,</span><span class="sxs-lookup"><span data-stu-id="10b45-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


