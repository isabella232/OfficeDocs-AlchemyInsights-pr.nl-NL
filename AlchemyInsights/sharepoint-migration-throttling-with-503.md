---
title: SharePoint-migratiebeperking met 503 fouten
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931653"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="19869-102">SharePoint-migratiebeperking met 503 fouten</span><span class="sxs-lookup"><span data-stu-id="19869-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="19869-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="19869-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="19869-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="19869-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="19869-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="19869-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="19869-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="19869-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="19869-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="19869-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="19869-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="19869-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="19869-109">**503 fouten bij het migreren naar SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="19869-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="19869-110">Het lijkt erop dat u migreert naar SharePoint Online en 503 fouten ontvangt.</span><span class="sxs-lookup"><span data-stu-id="19869-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="19869-111">Volg de onderstaande stappen zodat we u zo snel mogelijk kunnen helpen.</span><span class="sxs-lookup"><span data-stu-id="19869-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="19869-112">Klik **op Contact opnemen met ondersteuning**en vervolgens op Nieuwe **serviceaanvraag**.</span><span class="sxs-lookup"><span data-stu-id="19869-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="19869-113">Typ **SharePoint-migratiebeperking bij 503**voor de titel en beschrijving .</span><span class="sxs-lookup"><span data-stu-id="19869-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="19869-114">Zodra het ticket is ingediend, moet u het bijwerken met de volgende informatie:</span><span class="sxs-lookup"><span data-stu-id="19869-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="19869-115">Hoeveel migratie is er nog over (bijvoorbeeld hoeveel tbs?).</span><span class="sxs-lookup"><span data-stu-id="19869-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="19869-116">Begin- en einddatum migratie.</span><span class="sxs-lookup"><span data-stu-id="19869-116">Migration start and end date.</span></span>
    - <span data-ttu-id="19869-117">Beschrijf waar u uw inhoud migreert, zoals SharePoint Server, Box, GDrive, Bestandsshares, enz..</span><span class="sxs-lookup"><span data-stu-id="19869-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="19869-118">Schat het aantal beperkingsfouten (bijvoorbeeld x gaspedaal per uur?) en wanneer is de beperking gebeurd.</span><span class="sxs-lookup"><span data-stu-id="19869-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="19869-119">Welke migratietool u gebruikt (bijvoorbeeld SPMT of ShareGate).</span><span class="sxs-lookup"><span data-stu-id="19869-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


