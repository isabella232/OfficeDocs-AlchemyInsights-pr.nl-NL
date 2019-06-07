---
title: Beperk de toegang in de SharePoint- of OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759076"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fce4c-102">Beperk de toegang in de SharePoint- of OneDrive</span><span class="sxs-lookup"><span data-stu-id="fce4c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fce4c-103">Er zijn veel manieren om toegang te beperken tot SharePoint Online/OneDrive services.</span><span class="sxs-lookup"><span data-stu-id="fce4c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="fce4c-104">Deze verschillende methoden beperking worden hieronder nader belicht.</span><span class="sxs-lookup"><span data-stu-id="fce4c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="fce4c-105">Beperking van de machtiging</span><span class="sxs-lookup"><span data-stu-id="fce4c-105">Permission Restriction</span></span>

<span data-ttu-id="fce4c-106">In SharePoint Online en OneDrive voor Business beperken we toegang tot objecten, zoals sites, bestanden en mappen door alleen toegang verlenen tot de groepen/personen die toegang moeten hebben.</span><span class="sxs-lookup"><span data-stu-id="fce4c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="fce4c-107">Machtigingen voor een SharePoint-lijst of bibliotheek aanpassen</span><span class="sxs-lookup"><span data-stu-id="fce4c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="fce4c-108">Machtigingen voor SharePoint-site aanpassen</span><span class="sxs-lookup"><span data-stu-id="fce4c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="fce4c-109">De machtigingen voor een submap</span><span class="sxs-lookup"><span data-stu-id="fce4c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="fce4c-110">Toegang beheren vanaf niet-beheerde apparaten</span><span class="sxs-lookup"><span data-stu-id="fce4c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="fce4c-111">Als SharePoint of globale admin in Office 365, kunt u blokkeren of beperken van toegang tot SharePoint en OneDrive inhoud van niet-beheerde apparaten (die geen hybride AD gekoppelde of compatibele in Intune).</span><span class="sxs-lookup"><span data-stu-id="fce4c-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="fce4c-112">Netwerk locatie beperking</span><span class="sxs-lookup"><span data-stu-id="fce4c-112">Network Location Restriction</span></span>

<span data-ttu-id="fce4c-113">Als IT-beheer kunt u toegang tot bronnen van SharePoint en OneDrive op basis van gedefinieerde netwerklocaties die u vertrouwt.</span><span class="sxs-lookup"><span data-stu-id="fce4c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="fce4c-114">Dit is ook bekend als beleid op basis van locatie.</span><span class="sxs-lookup"><span data-stu-id="fce4c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="fce4c-115">Zie voor meer informatie, [toegang tot SharePoint Online en OneDrive gegevens op basis van locatie beheren](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="fce4c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="fce4c-116">Sitebeperking vergrendelen</span><span class="sxs-lookup"><span data-stu-id="fce4c-116">Site Lock Restriction</span></span> 

<span data-ttu-id="fce4c-117">U hebt de mogelijkheid een siteverzameling vergrendelen zodat niemand toegang heeft in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fce4c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="fce4c-118">Dit wordt ingesteld via PowerShell en [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met de eigenschap [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="fce4c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="fce4c-119">Voorkomen dat gebruikers kunnen sites of subsites maken</span><span class="sxs-lookup"><span data-stu-id="fce4c-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="fce4c-120">Als een beheerder van SharePoint of Office 365 globale beheerder kunt u uw gebruikers maken en beheren van hun eigen SharePoint-sites, bepalen wat voor soort sites kunnen maken, en geef de locatie van de sites.</span><span class="sxs-lookup"><span data-stu-id="fce4c-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="fce4c-121">Zie voor meer informatie, [maken van de site beheren in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="fce4c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

