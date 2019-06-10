---
title: Access services pensioen
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769432"
---
# <a name="access-services-retirement"></a><span data-ttu-id="aedd3-102">Access services pensioen</span><span class="sxs-lookup"><span data-stu-id="aedd3-102">Access services retirement</span></span>

<span data-ttu-id="aedd3-103">Zoals oorspronkelijk aangekondigd in MC97576, in maart 2017, en we communiceren in het afgelopen jaar wederom wordt toegang tot Services van Office 365 teruggetrokken.</span><span class="sxs-lookup"><span data-stu-id="aedd3-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="aedd3-104">De volgende fase in dit proces is het verwijderen van Databases van Access Web die SharePoint-lijsten als hun onderliggende gegevensopslag gebruiken.</span><span class="sxs-lookup"><span data-stu-id="aedd3-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="aedd3-105">**Wat betekent dit voor mij?**</span><span class="sxs-lookup"><span data-stu-id="aedd3-105">**How does this affect me?**</span></span>

<span data-ttu-id="aedd3-106">Begin juni 2019, we stoppen met het maken van een nieuwe Access-databases in SharePoint Online en de service en eventuele resterende apps afsluiten in April 2020.</span><span class="sxs-lookup"><span data-stu-id="aedd3-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="aedd3-107">**Wat moet ik doen als voorbereiding op deze wijziging?**</span><span class="sxs-lookup"><span data-stu-id="aedd3-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="aedd3-108">We raden u aan een overgang maken voor Access web-databases van de organisatie.</span><span class="sxs-lookup"><span data-stu-id="aedd3-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="aedd3-109">Beheerders kunt de [toegang tot SharePoint app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) ophalen een inventarisatie van de toegang tot toepassingen die door sites wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="aedd3-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="aedd3-110">Er zijn verschillende manieren om gegevens van Access web databases te migreren:</span><span class="sxs-lookup"><span data-stu-id="aedd3-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="aedd3-111">Importeren van een lokale Access-database (. ACCDB-bestand) of een Excel-bestand.</span><span class="sxs-lookup"><span data-stu-id="aedd3-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="aedd3-112">Ook wordt aangeraden Microsoft PowerApps verkennen als een alternatief platform zonder code zakelijke oplossingen voor web en mobiele apparaten maken.</span><span class="sxs-lookup"><span data-stu-id="aedd3-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>