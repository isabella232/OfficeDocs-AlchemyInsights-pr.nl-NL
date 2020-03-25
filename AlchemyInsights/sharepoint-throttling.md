---
title: SharePoint Online-beperking
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931437"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="34a83-102">SharePoint Online-beperking</span><span class="sxs-lookup"><span data-stu-id="34a83-102">SharePoint Online throttling</span></span>

<span data-ttu-id="34a83-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="34a83-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="34a83-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="34a83-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="34a83-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="34a83-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="34a83-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="34a83-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="34a83-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="34a83-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="34a83-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="34a83-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="34a83-109">**SharePoint Online-beperking**</span><span class="sxs-lookup"><span data-stu-id="34a83-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="34a83-110">SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden.</span><span class="sxs-lookup"><span data-stu-id="34a83-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="34a83-111">Beperking beperkt het aantal gebruikersacties of gelijktijdige aanroepen (per script of code) om overmatig gebruik van resources te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="34a83-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="34a83-112">Voor meer informatie u terecht op de onderstaande links.</span><span class="sxs-lookup"><span data-stu-id="34a83-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="34a83-113">Voorkomen dat u wordt beperkt of geblokkeerd in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="34a83-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="34a83-114">Gegevensmigratie en SPO-beperking</span><span class="sxs-lookup"><span data-stu-id="34a83-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="34a83-115">Migratiesnelheid van SharePoint Online en OneDrive</span><span class="sxs-lookup"><span data-stu-id="34a83-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="34a83-116">SharePoint Online-beperking verwerken door exponentiële back-off te gebruiken</span><span class="sxs-lookup"><span data-stu-id="34a83-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="34a83-117">Capaciteitsplanning en belastingtesten SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="34a83-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

