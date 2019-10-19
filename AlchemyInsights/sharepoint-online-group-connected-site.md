---
title: Een groep toevoegen aan een SharePoint-site
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750515"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="9917b-102">Problemen bij het maken of groeperen van verbonden sites in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9917b-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="9917b-103">Er zijn een aantal veelvoorkomende problemen opgetreden bij het maken of opnieuw maken van een groep verbonden site.</span><span class="sxs-lookup"><span data-stu-id="9917b-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="9917b-104">Als u een groep en de bijbehorende site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site definitief verwijderen.</span><span class="sxs-lookup"><span data-stu-id="9917b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="9917b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="9917b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="9917b-106">Zie voor meer informatie over aan de slag met PowerShell, aan de [slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="9917b-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="9917b-107">De site verwijderen uit verwijderde sites met behulp van de [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9917b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="9917b-108">Als u een groep verbonden site maakt en een waarschuwing ontvangt een andere groep met dezelfde alias al bestaat, controleert u de bestaande groepen van de [Office 365 vanuit het Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="9917b-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="9917b-109">U lost het probleem op door de bestaande groep te verwijderen als deze niet meer nodig is of de site te maken waaraan een andere alias is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="9917b-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="9917b-110">Er zijn verschillende manieren om moderne groepen met SharePoint te maken en te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="9917b-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="9917b-111">U bestaande sites verbinden met een Office 365-groep.</span><span class="sxs-lookup"><span data-stu-id="9917b-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="9917b-112">Zie [een Office 365-groep verbinden met de SharePoint-gebruiker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9917b-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="9917b-113">Als u een verbonden site van Office 365 groep wilt maken, moet u een team site maken.</span><span class="sxs-lookup"><span data-stu-id="9917b-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="9917b-114">Zie [een team site maken in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9917b-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

