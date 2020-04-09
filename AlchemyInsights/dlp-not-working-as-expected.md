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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977433"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5be34-102">DLP werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="5be34-102">DLP not working as expected</span></span>

<span data-ttu-id="5be34-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5be34-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="5be34-104">**DLP instellen**</span><span class="sxs-lookup"><span data-stu-id="5be34-104">**Setting up DLP**</span></span>

<span data-ttu-id="5be34-105">Heeft u problemen met **Data Loss Prevention (DLP)** in Office 365 werkt niet zoals verwacht?</span><span class="sxs-lookup"><span data-stu-id="5be34-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5be34-106">Zorg er dan voor dat uw **DLP-beleid** correct is ingesteld en dat uw gegevens bevatten waar het **DLP-beleid** naar op zoek is wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="5be34-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5be34-107">Met DLP-beleid u gevoelige informatie in uw organisatie identificeren en beveiligen.</span><span class="sxs-lookup"><span data-stu-id="5be34-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5be34-108">Als u DLP-beleid wilt instellen, gebruikt u de informatie [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="5be34-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5be34-109">**Waar dlp-beleid naar zoekt**</span><span class="sxs-lookup"><span data-stu-id="5be34-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5be34-110">Wanneer u de **ingebouwde gevoelige informatietypen** in het Office 365 Security and Compliance Center gebruikt, zoekt het DLP-beleid naar specifieke patronen en elementen bij het detecteren van deze gevoelige typen.</span><span class="sxs-lookup"><span data-stu-id="5be34-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5be34-111">**Ingebouwde gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="5be34-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5be34-112">Zie voor informatie over de ingebouwde gevoelige typen en waar een DLP-beleid naar zoekt bij het detecteren van het gevoelige type: [Waar de gevoelige informatietypen naar zoeken.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5be34-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5be34-113">**Aangepaste gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="5be34-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5be34-114">Als u aangepaste gevoelige informatietypen probeert te maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast gevoelig type: [Een aangepast gevoelig informatietype maken](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5be34-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5be34-115">**Een DLP-beleid testen**</span><span class="sxs-lookup"><span data-stu-id="5be34-115">**Test a DLP policy**</span></span>

<span data-ttu-id="5be34-116">Als u uw gegevens wilt testen met een ingebouwd of aangepast gevoelig informatietype, gebruikt u de optie **Testtype** onder**Gevoelige infotypen** **classificaties** > .</span><span class="sxs-lookup"><span data-stu-id="5be34-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5be34-117">Zie [Aangepaste gevoelige informatietypen testen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="5be34-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5be34-118">**Rapporten**</span><span class="sxs-lookup"><span data-stu-id="5be34-118">**Reports**</span></span>
  
- <span data-ttu-id="5be34-119">Krijg gevoelige gegevensinzichten met [DLP-rapporten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5be34-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5be34-120">Zie specifieke details van de gebeurtenis met een [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="5be34-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
