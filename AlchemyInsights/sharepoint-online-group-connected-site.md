---
title: Een groep toevoegen aan een SharePoint-site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642139"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="7d339-102">Problemen bij het maken van een met een groep verbonden site in SharePoint</span><span class="sxs-lookup"><span data-stu-id="7d339-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="7d339-103">Er zijn enkele veelvoorkomende problemen opgetreden bij het maken of opnieuw maken van een met een groep verbonden site.</span><span class="sxs-lookup"><span data-stu-id="7d339-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="7d339-104">Als u een groep en de bijbehorende site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site permanent verwijderen.</span><span class="sxs-lookup"><span data-stu-id="7d339-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="7d339-105">[SPO Management Shell downloaden](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="7d339-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="7d339-106">Zie [Aan de slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag met Powershell.</span><span class="sxs-lookup"><span data-stu-id="7d339-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="7d339-107">Verwijder de site uit verwijderde sites met de cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="7d339-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="7d339-108">Powershell is vereist om groepssites permanent te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="7d339-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="7d339-109">Als u een met een groep verbonden site maakt en een waarschuwing ontvangt: **een andere groep met dezelfde alias bestaat al,** controleert u de bestaande groepen in het Microsoft [365-beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="7d339-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="7d339-110">Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.</span><span class="sxs-lookup"><span data-stu-id="7d339-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="7d339-111">Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d339-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="7d339-112">U bestaande sites koppelen aan een Office 365-groep.</span><span class="sxs-lookup"><span data-stu-id="7d339-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="7d339-113">Zie [Een Office 365-groep verbinden met de gebruikersinterface van SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="7d339-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="7d339-114">Als u een site met office 365-groep wilt maken, moet u een [teamsite maken.](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="7d339-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
