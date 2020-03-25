---
title: DLP werkt niet zoals verwacht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932617"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="0c6ee-102">DLP werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="0c6ee-102">DLP not working as expected</span></span>

<span data-ttu-id="0c6ee-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0c6ee-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0c6ee-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0c6ee-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0c6ee-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0c6ee-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="0c6ee-109">**DLP instellen**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-109">**Setting up DLP**</span></span>

<span data-ttu-id="0c6ee-110">Heeft u problemen met **Data Loss Prevention (DLP)** in Office 365 werkt niet zoals verwacht?</span><span class="sxs-lookup"><span data-stu-id="0c6ee-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="0c6ee-111">Zorg er dan voor dat uw **DLP-beleid** correct is ingesteld en dat uw gegevens bevatten waar het **DLP-beleid** naar op zoek is wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="0c6ee-112">Met DLP-beleid u gevoelige informatie in uw organisatie identificeren en beveiligen.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="0c6ee-113">Als u DLP-beleid wilt instellen, gebruikt u de informatie [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="0c6ee-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="0c6ee-114">**Waar dlp-beleid naar zoekt**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="0c6ee-115">Wanneer u de **ingebouwde gevoelige informatietypen** in het Office 365 Security and Compliance Center gebruikt, zoekt het DLP-beleid naar specifieke patronen en elementen bij het detecteren van deze gevoelige typen.</span><span class="sxs-lookup"><span data-stu-id="0c6ee-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="0c6ee-116">**Ingebouwde gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="0c6ee-117">Zie voor informatie over de ingebouwde gevoelige typen en waar een DLP-beleid naar zoekt bij het detecteren van het gevoelige type: [Waar de gevoelige informatietypen naar zoeken.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0c6ee-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="0c6ee-118">**Aangepaste gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="0c6ee-119">Als u aangepaste gevoelige informatietypen probeert te maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast gevoelig type: [Een aangepast gevoelig informatietype maken](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0c6ee-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="0c6ee-120">**Een DLP-beleid testen**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-120">**Test a DLP policy**</span></span>

<span data-ttu-id="0c6ee-121">Als u uw gegevens wilt testen met een ingebouwd of aangepast gevoelig informatietype, gebruikt u de optie **Testtype** onder**Gevoelige infotypen** **classificaties** > .</span><span class="sxs-lookup"><span data-stu-id="0c6ee-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0c6ee-122">Zie [Aangepaste gevoelige informatietypen testen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="0c6ee-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="0c6ee-123">**Rapporten**</span><span class="sxs-lookup"><span data-stu-id="0c6ee-123">**Reports**</span></span>
  
- <span data-ttu-id="0c6ee-124">Krijg gevoelige gegevensinzichten met [DLP-rapporten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="0c6ee-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="0c6ee-125">Zie specifieke details van de gebeurtenis met een [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="0c6ee-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
