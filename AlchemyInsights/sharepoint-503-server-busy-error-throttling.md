---
title: SharePoint Online-beperking
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931221"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="8f6ae-102">SharePoint Online-beperking</span><span class="sxs-lookup"><span data-stu-id="8f6ae-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="8f6ae-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8f6ae-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8f6ae-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8f6ae-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8f6ae-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8f6ae-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8f6ae-109">**503-server is bezet fout**</span><span class="sxs-lookup"><span data-stu-id="8f6ae-109">**503 server is busy error**</span></span>

<span data-ttu-id="8f6ae-110">Gebruikers kunnen een 503-server ontvangen die een fout heeft wanneer ze naar SharePoint- of OneDrive-sites proberen te navigeren.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="8f6ae-111">Deze fout kan worden veroorzaakt door beperking binnen de SharePoint-service.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="8f6ae-112">SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="8f6ae-113">Beperking beperkt het aantal gebruikersacties of gelijktijdige aanroepen (per script of code) om overmatig gebruik van resources te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="8f6ae-114">Zie [Voorkomen dat u wordt beperkt of geblokkeerd in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)voor meer informatie over beperking.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="8f6ae-115">Als u van mening bent dat deze fout niets te maken heeft met beperking, u controleren of er actief onderhoud plaatsvindt op uw tenant door naar het [Berichtencentrum](https://portal.office.com/adminportal/home#/MessageCenter)te navigeren.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="8f6ae-116">Tot slot, zorg ervoor dat u de [pagina Service gezondheid](https://portal.office.com/adminportal/home#/servicehealth) om te controleren op eventuele adviezen / incidenten die zich kunnen voordoen.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

