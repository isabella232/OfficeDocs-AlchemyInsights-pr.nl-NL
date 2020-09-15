---
title: Toegang tot services buiten gebruik gesteld
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698677"
---
# <a name="access-services-retirement"></a><span data-ttu-id="74a28-102">Toegang tot services buiten gebruik gesteld</span><span class="sxs-lookup"><span data-stu-id="74a28-102">Access services retirement</span></span>

<span data-ttu-id="74a28-103">Aangezien we voor het eerst aangekondigd zijn in MC97576, in maart 2017, en de laatste keer dat de toegangs services van het afgelopen jaar wordt buiten gebruik gesteld.</span><span class="sxs-lookup"><span data-stu-id="74a28-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="74a28-104">De volgende fase van dit proces is de verwijdering van Access-webdatabases die SharePoint-lijsten gebruiken als onderliggende gegevensopslag.</span><span class="sxs-lookup"><span data-stu-id="74a28-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="74a28-105">**Wat betekent dit voor mij?**</span><span class="sxs-lookup"><span data-stu-id="74a28-105">**How does this affect me?**</span></span>

<span data-ttu-id="74a28-106">Vanaf 2019 wordt het maken van nieuwe Access-databases in SharePoint Online beëindigd en wordt de service en alle resterende apps van april 2020 uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="74a28-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="74a28-107">**Wat moet ik doen als voorbereiding op deze wijziging?**</span><span class="sxs-lookup"><span data-stu-id="74a28-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="74a28-108">U wordt aangeraden een overgangs plan te maken voor de Access-webdatabases van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="74a28-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="74a28-109">Beheerders kunnen de [app scanner van SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris van de Access-apps te verkrijgen die sites gebruiken.</span><span class="sxs-lookup"><span data-stu-id="74a28-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="74a28-110">Er zijn verschillende manieren om gegevens van Access-webdatabases te migreren:</span><span class="sxs-lookup"><span data-stu-id="74a28-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="74a28-111">Importeren in een lokale Access-database (. ACCDB) of een Excel-bestand.</span><span class="sxs-lookup"><span data-stu-id="74a28-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="74a28-112">We raden u ook aan om Microsoft PowerApps als een alternatief platform te ontwikkelen voor het maken van zakelijke oplossingen zonder code voor Internet en mobiele apparaten.</span><span class="sxs-lookup"><span data-stu-id="74a28-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>