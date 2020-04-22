---
title: Toegang tot diensten pensionering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687253"
---
# <a name="access-services-retirement"></a><span data-ttu-id="d2abf-102">Toegang tot diensten pensionering</span><span class="sxs-lookup"><span data-stu-id="d2abf-102">Access services retirement</span></span>

<span data-ttu-id="d2abf-103">Zoals we oorspronkelijk aangekondigd in MC97576, in maart 2017, en bleef communiceren in het afgelopen jaar Access Services worden teruggetrokken.</span><span class="sxs-lookup"><span data-stu-id="d2abf-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="d2abf-104">De volgende fase in dit proces is het verwijderen van Access Web Databases die SharePoint-lijsten gebruiken als onderliggende gegevensopslag.</span><span class="sxs-lookup"><span data-stu-id="d2abf-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="d2abf-105">**Wat voor invloed heeft dit op mij?**</span><span class="sxs-lookup"><span data-stu-id="d2abf-105">**How does this affect me?**</span></span>

<span data-ttu-id="d2abf-106">Vanaf juni 2019 stoppen we met het maken van nieuwe Access-databases in SharePoint Online en sluiten we de service en de resterende apps af in april 2020.</span><span class="sxs-lookup"><span data-stu-id="d2abf-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="d2abf-107">**Wat moet ik doen om me voor te bereiden op deze verandering?**</span><span class="sxs-lookup"><span data-stu-id="d2abf-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="d2abf-108">We raden u aan een overgangsplan te maken voor de Access-webdatabases van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="d2abf-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="d2abf-109">Beheerders kunnen de [SharePoint Access-app-scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris te krijgen van de Access-apps die sites gebruiken.</span><span class="sxs-lookup"><span data-stu-id="d2abf-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="d2abf-110">Er zijn verschillende manieren om Access-webdatabasesgegevens te migreren:</span><span class="sxs-lookup"><span data-stu-id="d2abf-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="d2abf-111">Importeren in een lokale Access-database (. ACCDB) of naar een Excel-bestand.</span><span class="sxs-lookup"><span data-stu-id="d2abf-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="d2abf-112">We raden u ook aan Microsoft PowerApps te verkennen als alternatief platform om bedrijfsno-codeoplossingen voor web- en mobiele apparaten te maken.</span><span class="sxs-lookup"><span data-stu-id="d2abf-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>