---
title: Toegang beperken in SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700450"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="bb265-102">Toegang beperken in SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="bb265-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="bb265-103">Er zijn verschillende manieren om toegang tot SharePoint Online/OneDrive-services te beperken.</span><span class="sxs-lookup"><span data-stu-id="bb265-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="bb265-104">Hieronder ziet u een overzicht van de verschillende restrictie methoden.</span><span class="sxs-lookup"><span data-stu-id="bb265-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="bb265-105">**Machtigingsbeperking**</span><span class="sxs-lookup"><span data-stu-id="bb265-105">**Permission Restriction**</span></span>

<span data-ttu-id="bb265-106">In SharePoint Online en OneDrive voor bedrijven beperkt u de toegang tot items, zoals sites, bestanden en mappen, alleen toegang tot de groepen en personen die toegang moeten hebben.</span><span class="sxs-lookup"><span data-stu-id="bb265-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="bb265-107">Machtigingen voor een SharePoint-lijst of-bibliotheek aanpassen</span><span class="sxs-lookup"><span data-stu-id="bb265-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="bb265-108">SharePoint-site machtigingen aanpassen</span><span class="sxs-lookup"><span data-stu-id="bb265-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="bb265-109">De machtigingen voor een submap wijzigen</span><span class="sxs-lookup"><span data-stu-id="bb265-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="bb265-110">Toegang beheren vanaf niet-beheerde apparaten</span><span class="sxs-lookup"><span data-stu-id="bb265-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="bb265-111">Als SharePoint-of globale beheerder kunt u de toegang tot SharePoint-en OneDrive-inhoud van niet-beheerde apparaten blokkeren of beperken (niet-hybride aantekening of compatibel met intune).</span><span class="sxs-lookup"><span data-stu-id="bb265-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="bb265-112">**Beperking van netwerklocatie**</span><span class="sxs-lookup"><span data-stu-id="bb265-112">**Network Location Restriction**</span></span>

<span data-ttu-id="bb265-113">Als IT-beheerder kunt u de toegang tot SharePoint-en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt.</span><span class="sxs-lookup"><span data-stu-id="bb265-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="bb265-114">Dit wordt ook wel het beleid op basis van locatie genoemd.</span><span class="sxs-lookup"><span data-stu-id="bb265-114">This is also known as location-based policy.</span></span> <span data-ttu-id="bb265-115">Zie [toegang tot SharePoint Online en OneDrive-gegevens beheren op basis van netwerklocatie](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="bb265-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="bb265-116">**Beperking site vergrendeling**</span><span class="sxs-lookup"><span data-stu-id="bb265-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="bb265-117">In SharePoint Online kunt u de mogelijkheid van een siteverzameling vergrendelen, zodat niemand toegang heeft.</span><span class="sxs-lookup"><span data-stu-id="bb265-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="bb265-118">Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de eigenschap [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="bb265-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="bb265-119">**Voorkomen dat gebruikers sites of subsites maken**</span><span class="sxs-lookup"><span data-stu-id="bb265-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="bb265-120">Als SharePoint-beheerder of globale beheerder kunt u toestaan dat uw gebruikers hun eigen SharePoint-sites maken en beheren, bepalen welke soorten sites ze kunnen maken en de locatie van de sites opgeven.</span><span class="sxs-lookup"><span data-stu-id="bb265-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="bb265-121">Zie [sites maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="bb265-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

