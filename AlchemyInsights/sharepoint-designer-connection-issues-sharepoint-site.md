---
title: Verbindingsproblemen met SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051708"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="da150-102">Verbindingsproblemen met SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="da150-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="da150-103">Als SharePoint Designer verbindingsproblemen ondervindt met SharePoint-sites, probeert u de volgende algemene oplossingen.</span><span class="sxs-lookup"><span data-stu-id="da150-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="da150-104">Stap 1: Controleer of SharePoint Designer 2013 is bijgewerkt met [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) en de [Update 2, 2016 voorsharepoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="da150-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="da150-105">Stap 2: wis de lokale cachebestanden:</span><span class="sxs-lookup"><span data-stu-id="da150-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="da150-106">Sluit SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="da150-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="da150-107">Verwijder alle bestanden die in de volgende mappen zijn gevonden op de lokale computer.</span><span class="sxs-lookup"><span data-stu-id="da150-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="da150-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="da150-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="da150-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="da150-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="da150-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="da150-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="da150-111">Open SharePoint Designer 2013 en voer het account opnieuw in om te zien of het werkt.</span><span class="sxs-lookup"><span data-stu-id="da150-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="da150-112">Stap 3: [Schakel moderne verificatie voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="da150-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="da150-113">Stap 4: beheerders moeten het **aangepaste script toestaan** in de instellingen van het SharePoint Admin Center om de SharePoint Designer-verbinding toe te staan.</span><span class="sxs-lookup"><span data-stu-id="da150-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="da150-114">Zie [aangepast script toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="da150-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


