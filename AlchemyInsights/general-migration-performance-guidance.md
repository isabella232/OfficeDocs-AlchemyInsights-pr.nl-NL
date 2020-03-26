---
title: Algemene richtlijnen voor migratieprestaties
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932474"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="862d5-102">Algemene richtlijnen voor migratieprestaties</span><span class="sxs-lookup"><span data-stu-id="862d5-102">General migration performance guidance</span></span>

<span data-ttu-id="862d5-103">**Belangrijk**: Veel klanten met SharePoint Online en OneDrive voeren bedrijfskritische toepassingen uit op de service die op de achtergrond worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="862d5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="862d5-104">Dit zijn onder andere het migreren van inhoud, de preventie van gegevensverlies (DLP) en back-up-oplossingen.</span><span class="sxs-lookup"><span data-stu-id="862d5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="862d5-105">Tijdens deze ongekende tijden worden er stappen ondernomen om ervoor te zorgen dat de SharePoint Online-en OneDrive-services beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van werken op afstand.</span><span class="sxs-lookup"><span data-stu-id="862d5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="862d5-106">Ter ondersteuning van dit doel hebben we strengere limieten geïmplementeerd voor de achtergrond-apps (migratie, DLP-en back-up-oplossing) overdag gedurende weekdagen.</span><span class="sxs-lookup"><span data-stu-id="862d5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="862d5-107">U kunt verwachten dat deze apps zeer beperkte doorvoercapaciteit hebben gedurende deze momenten.</span><span class="sxs-lookup"><span data-stu-id="862d5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="862d5-108">Tijdens avond-en weekenduren voor de regio is de service echter gereed voor het verwerken van een aanzienlijk grotere hoeveelheid aanvragen van de achtergrond-apps.</span><span class="sxs-lookup"><span data-stu-id="862d5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="862d5-109">**Richtlijnen voor migratieprestaties**</span><span class="sxs-lookup"><span data-stu-id="862d5-109">**Migration performance guidance**</span></span>

<span data-ttu-id="862d5-110">Migratieprestaties kunnen worden beïnvloed door netwerkinfrastructuur, bestandsgrootte, migratietijd en beperking.</span><span class="sxs-lookup"><span data-stu-id="862d5-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="862d5-111">Een beter begrip van deze factoren kan u helpen bij het plannen en maximaliseren van een efficiënte migratie.</span><span class="sxs-lookup"><span data-stu-id="862d5-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="862d5-112">Algemene richtlijnen voor migratieprestaties</span><span class="sxs-lookup"><span data-stu-id="862d5-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
