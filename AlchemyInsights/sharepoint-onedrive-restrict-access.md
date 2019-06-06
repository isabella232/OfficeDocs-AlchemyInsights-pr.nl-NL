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
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735138"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="18500-102">Beperk de toegang in de SharePoint- of OneDrive</span><span class="sxs-lookup"><span data-stu-id="18500-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="18500-103">Er zijn veel manieren om toegang te beperken tot SharePoint Online/OneDrive services.</span><span class="sxs-lookup"><span data-stu-id="18500-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="18500-104">Deze verschillende methoden beperking worden hieronder nader belicht.</span><span class="sxs-lookup"><span data-stu-id="18500-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="18500-105">Beperking van de machtiging</span><span class="sxs-lookup"><span data-stu-id="18500-105">Permission Restriction</span></span>

<span data-ttu-id="18500-106">In SharePoint Online en OneDrive voor Business beperken we toegang tot objecten, zoals sites, bestanden en mappen door alleen toegang verlenen tot de groepen/personen die toegang moeten hebben.</span><span class="sxs-lookup"><span data-stu-id="18500-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="18500-107">Machtigingen voor een SharePoint-lijst of bibliotheek aanpassen</span><span class="sxs-lookup"><span data-stu-id="18500-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="18500-108">Machtigingen voor SharePoint-site aanpassen</span><span class="sxs-lookup"><span data-stu-id="18500-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="18500-109">De machtigingen voor een submap</span><span class="sxs-lookup"><span data-stu-id="18500-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="18500-110">Toegang beheren vanaf niet-beheerde apparaten</span><span class="sxs-lookup"><span data-stu-id="18500-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="18500-111">Als SharePoint of globale admin in Office 365, kunt u blokkeren of beperken van toegang tot SharePoint en OneDrive inhoud van niet-beheerde apparaten (die geen hybride AD gekoppelde of compatibele in Intune).</span><span class="sxs-lookup"><span data-stu-id="18500-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="18500-112">Netwerk locatie beperking</span><span class="sxs-lookup"><span data-stu-id="18500-112">Network Location Restriction</span></span>

<span data-ttu-id="18500-113">Als IT-beheer kunt u toegang tot bronnen van SharePoint en OneDrive op basis van gedefinieerde netwerklocaties die u vertrouwt.</span><span class="sxs-lookup"><span data-stu-id="18500-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="18500-114">Dit is ook bekend als beleid op basis van locatie.</span><span class="sxs-lookup"><span data-stu-id="18500-114">This is also known as location-based policy.</span></span> <span data-ttu-id="18500-115">Zie voor meer informatie, [toegang tot SharePoint Online en OneDrive gegevens op basis van locatie beheren](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="18500-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="18500-116">Sitebeperking vergrendelen</span><span class="sxs-lookup"><span data-stu-id="18500-116">Site Lock Restriction</span></span> 

<span data-ttu-id="18500-117">U hebt de mogelijkheid een siteverzameling vergrendelen zodat niemand toegang heeft in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="18500-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="18500-118">Dit wordt ingesteld via PowerShell en [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met de eigenschap [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="18500-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="18500-119">Voorkomen dat gebruikers kunnen sites of subsites maken</span><span class="sxs-lookup"><span data-stu-id="18500-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="18500-120">Als een beheerder van SharePoint of Office 365 globale beheerder kunt u uw gebruikers maken en beheren van hun eigen SharePoint-sites, bepalen wat voor soort sites kunnen maken, en geef de locatie van de sites.</span><span class="sxs-lookup"><span data-stu-id="18500-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="18500-121">Zie voor meer informatie, [maken van de site beheren in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="18500-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

