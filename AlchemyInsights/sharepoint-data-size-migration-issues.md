---
title: Problemen tijdens het migreren van gegevens naar SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931689"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="c7013-102">Problemen tijdens het migreren van gegevens naar SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c7013-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="c7013-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="c7013-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c7013-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="c7013-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c7013-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="c7013-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c7013-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="c7013-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c7013-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="c7013-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c7013-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="c7013-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c7013-109">**Meer dan 100 TB aan gegevens migreren**</span><span class="sxs-lookup"><span data-stu-id="c7013-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="c7013-110">Het lijkt erop dat u meer dan 100 TB aan gegevens migreert naar SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c7013-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="c7013-111">Volg de onderstaande stappen zodat we u zo snel mogelijk kunnen helpen.</span><span class="sxs-lookup"><span data-stu-id="c7013-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="c7013-112">Selecteer **Nieuwe serviceaanvraag**en vervolgens **Nieuwe serviceaanvraag**.</span><span class="sxs-lookup"><span data-stu-id="c7013-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="c7013-113">Laat de titel en beschrijving als **SharePoint-migratie van meer dan 100 TB .**</span><span class="sxs-lookup"><span data-stu-id="c7013-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="c7013-114">Zodra het ticket is ingediend, moet u het bijwerken met de volgende informatie:</span><span class="sxs-lookup"><span data-stu-id="c7013-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="c7013-115">Geschatte grootte van uw migratie.</span><span class="sxs-lookup"><span data-stu-id="c7013-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="c7013-116">Een schatting van wanneer u uw migratie wilt starten en voltooien.</span><span class="sxs-lookup"><span data-stu-id="c7013-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="c7013-117">Beschrijf waar u uw inhoud migreert, zoals SharePoint Server, Box, GDrive, Bestandsshares, enz..</span><span class="sxs-lookup"><span data-stu-id="c7013-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

