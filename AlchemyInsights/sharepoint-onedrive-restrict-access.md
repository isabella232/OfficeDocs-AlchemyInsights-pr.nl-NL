---
title: Toegang beperken in SharePoint of OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750659"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="05ba6-102">Toegang beperken in SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="05ba6-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="05ba6-103">Er zijn veel manieren om de toegang tot SharePoint Online/OneDrive-services te beperken.</span><span class="sxs-lookup"><span data-stu-id="05ba6-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="05ba6-104">Deze verschillende methoden voor toegangsbeperking worden hieronder beschreven.</span><span class="sxs-lookup"><span data-stu-id="05ba6-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="05ba6-105">**Beperking van machtigingen**</span><span class="sxs-lookup"><span data-stu-id="05ba6-105">**Permission Restriction**</span></span>

<span data-ttu-id="05ba6-106">In SharePoint Online en OneDrive voor bedrijven beperken we de toegang tot items zoals sites, bestanden en mappen door alleen toegang te verlenen aan die groepen/personen die toegang moeten hebben.</span><span class="sxs-lookup"><span data-stu-id="05ba6-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="05ba6-107">Machtigingen voor een SharePoint-lijst of-bibliotheek aanpassen</span><span class="sxs-lookup"><span data-stu-id="05ba6-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="05ba6-108">SharePoint-site machtigingen aanpassen</span><span class="sxs-lookup"><span data-stu-id="05ba6-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="05ba6-109">De machtigingen voor een submap wijzigen</span><span class="sxs-lookup"><span data-stu-id="05ba6-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="05ba6-110">Toegang beheren vanaf niet-beheerde apparaten</span><span class="sxs-lookup"><span data-stu-id="05ba6-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="05ba6-111">Als een SharePoint of globale beheerder in Office 365, u blokkeren of beperken van toegang tot SharePoint en OneDrive-inhoud van niet-beheerde apparaten (die niet hybride AD toegevoegd of compatibel zijn in intune).</span><span class="sxs-lookup"><span data-stu-id="05ba6-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="05ba6-112">**Beperking van netwerklocatie**</span><span class="sxs-lookup"><span data-stu-id="05ba6-112">**Network Location Restriction**</span></span>

<span data-ttu-id="05ba6-113">Als IT-beheerder u de toegang tot SharePoint-en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt.</span><span class="sxs-lookup"><span data-stu-id="05ba6-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="05ba6-114">Dit wordt ook wel op locatie gebaseerd beleid genoemd.</span><span class="sxs-lookup"><span data-stu-id="05ba6-114">This is also known as location-based policy.</span></span> <span data-ttu-id="05ba6-115">Voor meer informatie raadpleegt u [toegang tot SharePoint Online en OneDrive-gegevens beheren op basis van netwerklocatie](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="05ba6-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="05ba6-116">**Beperking van site vergrendeling**</span><span class="sxs-lookup"><span data-stu-id="05ba6-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="05ba6-117">In SharePoint Online hebt u de mogelijkheid om een siteverzameling te vergrendelen, zodat niemand toegang heeft.</span><span class="sxs-lookup"><span data-stu-id="05ba6-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="05ba6-118">Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate eigenschap.</span><span class="sxs-lookup"><span data-stu-id="05ba6-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="05ba6-119">**Gebruikers beperken om sites of subsites te maken**</span><span class="sxs-lookup"><span data-stu-id="05ba6-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="05ba6-120">Als SharePoint-beheerder of Office 365 globale beheerder u uw gebruikers hun eigen SharePoint-sites laten maken en beheren, bepalen wat voor soort sites ze kunnen maken en de locatie van de sites opgeven.</span><span class="sxs-lookup"><span data-stu-id="05ba6-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="05ba6-121">Zie voor meer informatie, [site maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="05ba6-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

