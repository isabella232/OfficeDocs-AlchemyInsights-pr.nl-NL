---
title: Toegang in SharePoint of OneDrive beperken
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692760"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="04fb0-102">Toegang in SharePoint of OneDrive beperken</span><span class="sxs-lookup"><span data-stu-id="04fb0-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="04fb0-103">Er zijn veel manieren om de toegang tot SharePoint Online/OneDrive-services te beperken.</span><span class="sxs-lookup"><span data-stu-id="04fb0-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="04fb0-104">Deze verschillende toegangsbeperkingsmethoden worden hieronder beschreven.</span><span class="sxs-lookup"><span data-stu-id="04fb0-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="04fb0-105">**Machtigingsbeperking**</span><span class="sxs-lookup"><span data-stu-id="04fb0-105">**Permission Restriction**</span></span>

<span data-ttu-id="04fb0-106">In SharePoint Online en OneDrive voor Bedrijven beperken we de toegang tot items zoals sites, bestanden en mappen door alleen toegang te verlenen aan groepen/personen die toegang moeten hebben.</span><span class="sxs-lookup"><span data-stu-id="04fb0-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="04fb0-107">Machtigingen aanpassen voor een SharePoint-lijst of -bibliotheek</span><span class="sxs-lookup"><span data-stu-id="04fb0-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="04fb0-108">SharePoint-site machtigingen aanpassen</span><span class="sxs-lookup"><span data-stu-id="04fb0-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="04fb0-109">De machtigingen voor een submap wijzigen</span><span class="sxs-lookup"><span data-stu-id="04fb0-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="04fb0-110">Toegang beheren vanaf niet-beheerde apparaten</span><span class="sxs-lookup"><span data-stu-id="04fb0-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="04fb0-111">Als SharePoint- of globale beheerder u de toegang tot SharePoint- en OneDrive-inhoud vanaf niet-beheerde apparaten blokkeren of beperken (die niet hybride AD hebben samengevoegd of in Intune zijn compatibel).</span><span class="sxs-lookup"><span data-stu-id="04fb0-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="04fb0-112">**Beperking van de netwerklocatie**</span><span class="sxs-lookup"><span data-stu-id="04fb0-112">**Network Location Restriction**</span></span>

<span data-ttu-id="04fb0-113">Als IT-beheerder u de toegang tot SharePoint- en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt.</span><span class="sxs-lookup"><span data-stu-id="04fb0-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="04fb0-114">Dit wordt ook wel locatiegebaseerd beleid genoemd.</span><span class="sxs-lookup"><span data-stu-id="04fb0-114">This is also known as location-based policy.</span></span> <span data-ttu-id="04fb0-115">Zie Toegang tot [SharePoint Online- en OneDrive-gegevens](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) beheren op basis van netwerklocatie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="04fb0-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="04fb0-116">**Beperking sitevergrendeling**</span><span class="sxs-lookup"><span data-stu-id="04fb0-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="04fb0-117">Binnen SharePoint Online hebt u de mogelijkheid om een siteverzameling te vergrendelen, zodat niemand toegang heeft.</span><span class="sxs-lookup"><span data-stu-id="04fb0-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="04fb0-118">Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de eigenschap [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="04fb0-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="04fb0-119">**Gebruikers beperken om sites of subsites te maken**</span><span class="sxs-lookup"><span data-stu-id="04fb0-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="04fb0-120">Als SharePoint-beheerder of globale beheerder u uw gebruikers hun eigen SharePoint-sites laten maken en beheren, bepalen wat voor soort sites ze kunnen maken en de locatie van de sites opgeven.</span><span class="sxs-lookup"><span data-stu-id="04fb0-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="04fb0-121">Zie [Sitemaken van de site beheren in SharePoint Online beheren voor](https://docs.microsoft.com/sharepoint/manage-site-creation) meer informatie</span><span class="sxs-lookup"><span data-stu-id="04fb0-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

