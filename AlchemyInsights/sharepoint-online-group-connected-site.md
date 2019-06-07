---
title: Een groep toevoegen aan een SharePoint-site
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758726"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="f8db7-102">Groep verbonden site in SharePoint Online maken</span><span class="sxs-lookup"><span data-stu-id="f8db7-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="f8db7-103">Er zijn een aantal veelvoorkomende problemen opgetreden bij het maken van of opnieuw een groep site verbonden.</span><span class="sxs-lookup"><span data-stu-id="f8db7-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="f8db7-104">Als u een groep en haar verbonden site hebt verwijderd en een andere site te maken met dezelfde URL, moet u de vorige site permanent te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="f8db7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="f8db7-105">[Gesimuleerde Productieorder Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) downloaden</span><span class="sxs-lookup"><span data-stu-id="f8db7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="f8db7-106">Zie voor meer informatie over aan de slag met powershell, [aan de slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="f8db7-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="f8db7-107">De Site verwijderen uit Verwijderde Sites met behulp van de powershell-cmdlet [Verwijderen SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="f8db7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="f8db7-108">Als u een groep verbonden site maakt en u ontvangt een waarschuwing bestaat al een groep met dezelfde alias, controleert u de bestaande groepen uit de [Office 365 vanuit de Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="f8db7-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="f8db7-109">Het probleem is opgelost, de bestaande groep verwijderen als deze niet meer nodig is of de site maken met een ander alias toegewezen.</span><span class="sxs-lookup"><span data-stu-id="f8db7-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="f8db7-110">Er zijn verschillende manieren maken en moderne groepen gebruiken met SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f8db7-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="f8db7-111">U kunt bestaande sites verbinden met een Office 365-groep.</span><span class="sxs-lookup"><span data-stu-id="f8db7-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="f8db7-112">Zie [verbinding maken met een Office 365-groep met de SharePoint gebruiker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer info.</span><span class="sxs-lookup"><span data-stu-id="f8db7-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="f8db7-113">Als een Office 365 groep verbonden site maakt, moet u een Team Site te maken.</span><span class="sxs-lookup"><span data-stu-id="f8db7-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="f8db7-114">Zie voor meer info, [een team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="f8db7-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

