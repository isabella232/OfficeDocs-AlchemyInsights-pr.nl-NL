---
title: Toegang tot pensioendiensten
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747779"
---
# <a name="access-services-retirement"></a><span data-ttu-id="7b567-102">Toegang tot pensioendiensten</span><span class="sxs-lookup"><span data-stu-id="7b567-102">Access services retirement</span></span>

<span data-ttu-id="7b567-103">Zoals we oorspronkelijk aankondigden in MC97576, in maart 2017, en bleven communiceren over het afgelopen jaar, worden de toegangsdiensten buiten gebruik gesteld van Office 365.</span><span class="sxs-lookup"><span data-stu-id="7b567-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="7b567-104">De volgende fase in dit proces is het verwijderen van Access Web-databases die gebruikmaken van SharePoint-lijsten als onderliggende gegevensopslag.</span><span class="sxs-lookup"><span data-stu-id="7b567-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="7b567-105">**Hoe beïnvloedt dit mij?**</span><span class="sxs-lookup"><span data-stu-id="7b567-105">**How does this affect me?**</span></span>

<span data-ttu-id="7b567-106">Vanaf juni 2019 zullen we stoppen met het maken van nieuwe Access-databases in SharePoint Online en de service en eventuele resterende apps afsluiten door 2020 april.</span><span class="sxs-lookup"><span data-stu-id="7b567-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="7b567-107">**Wat moet ik doen om voor te bereiden op deze wijziging?**</span><span class="sxs-lookup"><span data-stu-id="7b567-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="7b567-108">We raden u aan een overgangsplan voor de Access-webdatabases van uw organisatie te maken.</span><span class="sxs-lookup"><span data-stu-id="7b567-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="7b567-109">Beheerders kunnen de [SharePoint Access app-scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris op te vragen van de Access-apps die sites gebruiken.</span><span class="sxs-lookup"><span data-stu-id="7b567-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="7b567-110">Er zijn verschillende manieren om gegevens van Access-webdatabases te migreren:</span><span class="sxs-lookup"><span data-stu-id="7b567-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="7b567-111">Importeren in een lokale Access-database (. ACCDB) of naar een Excel-bestand.</span><span class="sxs-lookup"><span data-stu-id="7b567-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="7b567-112">We raden u ook aan Microsoft PowerApps te verkennen als alternatief platform voor het maken van niet-code zakelijke oplossingen voor web-en mobiele apparaten.</span><span class="sxs-lookup"><span data-stu-id="7b567-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>