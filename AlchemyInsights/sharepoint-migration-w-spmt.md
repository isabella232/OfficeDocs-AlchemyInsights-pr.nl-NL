---
title: SharePoint-migratie met SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931545"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="8d84a-102">SharePoint-migratie met SPMT</span><span class="sxs-lookup"><span data-stu-id="8d84a-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="8d84a-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="8d84a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8d84a-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="8d84a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8d84a-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="8d84a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8d84a-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="8d84a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8d84a-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="8d84a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8d84a-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="8d84a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8d84a-109">**SharePoint-migratieprogramma**</span><span class="sxs-lookup"><span data-stu-id="8d84a-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="8d84a-110">De SharePoint Migration Tool is ontworpen om te worden gebruikt voor migraties variërend van de kleinste set bestanden tot een grootschalige bedrijfsmigratie, en stelt u in staat om uw gegevens over te zetten naar de cloud en te profiteren van de nieuwste samenwerking, intelligentie en beveiligingsoplossingen met Office 365.</span><span class="sxs-lookup"><span data-stu-id="8d84a-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="8d84a-111">Het SharePoint-migratiehulpprogramma downloaden en installeren</span><span class="sxs-lookup"><span data-stu-id="8d84a-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="8d84a-112">Problemen en fouten met veelvoorkomende SPMT-problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="8d84a-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="8d84a-113">Problemen met spmt-installatie oplossen</span><span class="sxs-lookup"><span data-stu-id="8d84a-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
