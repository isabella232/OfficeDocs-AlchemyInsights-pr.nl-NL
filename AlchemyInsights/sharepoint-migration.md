---
title: Opties migreren naar SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932725"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="f517b-102">Opties migreren naar SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f517b-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="f517b-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="f517b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f517b-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="f517b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f517b-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="f517b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f517b-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="f517b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f517b-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="f517b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f517b-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="f517b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f517b-109">**Migratieopties**</span><span class="sxs-lookup"><span data-stu-id="f517b-109">**Migration options**</span></span>

<span data-ttu-id="f517b-110">Er zijn verschillende opties beschikbaar om inhoud te migreren naar SharePoint Online, afhankelijk van de grootte en hoeveelheid bestanden die u moet verplaatsen, raadpleegt u [hier](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)een lijst met opties.</span><span class="sxs-lookup"><span data-stu-id="f517b-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="f517b-111">Ga voor meer informatie over contentmigratie naar de onderstaande links.</span><span class="sxs-lookup"><span data-stu-id="f517b-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="f517b-112">Sharepoint-migratiehulpprogramma</span><span class="sxs-lookup"><span data-stu-id="f517b-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="f517b-113">Aan de slag met de migratiemanager</span><span class="sxs-lookup"><span data-stu-id="f517b-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="f517b-114">Migratiesnelheid van Sharepoint Online en ODB</span><span class="sxs-lookup"><span data-stu-id="f517b-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="f517b-115">Voorkomen dat u wordt beperkt of geblokkeerd in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f517b-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f517b-116">SharePoint Migration Assessment Tool (SMAT)</span><span class="sxs-lookup"><span data-stu-id="f517b-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="f517b-117">**Opmerking:** momenteel ondersteunt het sharepointmigratiehulpprogramma alleen migraties vanuit SharePoint 2010 en 2013.</span><span class="sxs-lookup"><span data-stu-id="f517b-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="f517b-118">Versie 2016 of 2019 wordt op dit moment niet ondersteund.</span><span class="sxs-lookup"><span data-stu-id="f517b-118">Version 2016 or 2019 are not supported at this time.</span></span>
