---
title: Problemen en fouten van SharePoint-migratiehulpprogramma's oplossen
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931113"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="23f6a-102">Problemen en fouten van SharePoint-migratiehulpprogramma's oplossen</span><span class="sxs-lookup"><span data-stu-id="23f6a-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="23f6a-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="23f6a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="23f6a-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="23f6a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="23f6a-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="23f6a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="23f6a-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="23f6a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="23f6a-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="23f6a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="23f6a-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="23f6a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="23f6a-109">**Veelvoorkomende problemen en fouten**</span><span class="sxs-lookup"><span data-stu-id="23f6a-109">**Common issues and errors**</span></span>

<span data-ttu-id="23f6a-110">U een aantal veelvoorkomende problemen en fouten tegenkomen bij het gebruik van het SharePoint Migration Tool (SPMT).</span><span class="sxs-lookup"><span data-stu-id="23f6a-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="23f6a-111">Raadpleeg de onderstaande links voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="23f6a-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="23f6a-112">Problemen en fouten met veelvoorkomende SPMT-problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="23f6a-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="23f6a-113">Problemen met het oplossen van problemen met het installeren van SPMT oplossen</span><span class="sxs-lookup"><span data-stu-id="23f6a-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)