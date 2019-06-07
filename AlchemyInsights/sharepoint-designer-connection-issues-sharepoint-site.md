---
title: Machtigingsniveaus voor SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760688"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="1424c-102">Problemen met SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="1424c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="1424c-103">Als u SharePoint Designer ondervindt problemen met de verbinding met de SharePoint-sites, probeer dan de volgende gemeenschappelijke oplossingen.</span><span class="sxs-lookup"><span data-stu-id="1424c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="1424c-104">Stap 1: Controleer of SharePoint Designer wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="1424c-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="1424c-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="1424c-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="1424c-106">Servicepack 1 (SP1) voor SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="1424c-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="1424c-107">Update voor SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="1424c-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="1424c-108">Stap 2: Wis de bestanden in de lokale cache</span><span class="sxs-lookup"><span data-stu-id="1424c-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="1424c-109">Sluit de SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="1424c-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="1424c-110">Ga naar de volgende mappen te verwijderen van bestanden in de cache op de lokale computer.</span><span class="sxs-lookup"><span data-stu-id="1424c-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="1424c-111">Klik op Start, uitvoeren en verwijderen, alle bestanden in elk van gevonden de onderstaande locaties.</span><span class="sxs-lookup"><span data-stu-id="1424c-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="1424c-112">%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="1424c-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="1424c-113">SharePoint Designer 2013 openen en geef de account opnieuw om te zien als het werkt.</span><span class="sxs-lookup"><span data-stu-id="1424c-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="1424c-114">Stap 3: [moderne voor Office 2013 op apparaten met Windows-verificatie inschakelen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="1424c-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="1424c-115">Stap 4: Beheerders moet aangepast Script dat de verbinding van SharePoint Designer toestaan.</span><span class="sxs-lookup"><span data-stu-id="1424c-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="1424c-116">Zie voor gedetailleerde stappen, voorbeelden en overwegingen [toestaan of voorkomen van aangepast script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="1424c-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


