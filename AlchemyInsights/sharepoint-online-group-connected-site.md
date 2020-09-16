---
title: Een groep toevoegen aan een SharePoint-site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771194"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="00b7b-102">Problemen bij het maken van een met een groep verbonden site in SharePoint</span><span class="sxs-lookup"><span data-stu-id="00b7b-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="00b7b-103">Enkele veelvoorkomende problemen die kunnen optreden bij het maken of opnieuw maken van een verbonden groepssite.</span><span class="sxs-lookup"><span data-stu-id="00b7b-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="00b7b-104">Als u een groep en de gekoppelde site hebt verwijderd en een andere site wilt maken met dezelfde URL, moet u de vorige site permanent verwijderen.</span><span class="sxs-lookup"><span data-stu-id="00b7b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="00b7b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="00b7b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="00b7b-106">Zie aan de slag [met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag met PowerShell.</span><span class="sxs-lookup"><span data-stu-id="00b7b-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="00b7b-107">Verwijder de site van verwijderde sites met behulp van de PowerShell [-cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="00b7b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="00b7b-108">PowerShell is vereist voor het permanent verwijderen van groeps sites.</span><span class="sxs-lookup"><span data-stu-id="00b7b-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="00b7b-109">Als u een site met een groep wilt maken en een waarschuwing wilt ontvangen: er **bestaat al een andere groep met dezelfde alias**, Controleer de bestaande groepen in het [Microsoft 365-Beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="00b7b-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="00b7b-110">Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.</span><span class="sxs-lookup"><span data-stu-id="00b7b-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="00b7b-111">U kunt moderne groepen met SharePoint op verschillende manieren maken en gebruiken.</span><span class="sxs-lookup"><span data-stu-id="00b7b-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="00b7b-112">U kunt bestaande sites verbinden met een Microsoft 365-groep.</span><span class="sxs-lookup"><span data-stu-id="00b7b-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="00b7b-113">Zie [een Microsoft 365-groep verbinden met de gebruikersinterface van SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="00b7b-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="00b7b-114">Als u een site met een Microsoft 365-groep wilt maken, moet u een [team site](https://admin.microsoft.com/sharepoint)maken.</span><span class="sxs-lookup"><span data-stu-id="00b7b-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
