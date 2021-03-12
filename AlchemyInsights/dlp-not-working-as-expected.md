---
title: DLP werkt niet zoals verwacht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707805"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e627a-102">DLP werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="e627a-102">DLP not working as expected</span></span>

<span data-ttu-id="e627a-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e627a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e627a-104">**DLP instellen**</span><span class="sxs-lookup"><span data-stu-id="e627a-104">**Setting up DLP**</span></span>

<span data-ttu-id="e627a-105">Werkt de preventie van gegevensverlies **(DLP)** in Office 365 niet zoals verwacht?</span><span class="sxs-lookup"><span data-stu-id="e627a-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e627a-106">Zo ja, zorg er dan voor dat uw **DLP-beleid** juist is ingesteld en dat uw gegevens bevatten waar het **DLP-beleid** naar zoekt wanneer dit wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="e627a-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e627a-107">Met DLP-beleid kunt u gevoelige informatie in uw organisatie identificeren en beveiligen.</span><span class="sxs-lookup"><span data-stu-id="e627a-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e627a-108">Gebruik de informatie hier voor het instellen van [DLP-beleidsregels.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="e627a-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="e627a-109">**Waar wordt naar ged zoeken met DLP-beleid**</span><span class="sxs-lookup"><span data-stu-id="e627a-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e627a-110">Wanneer u de ingebouwde typen gevoelige informatie in het Beveiligings- en compliancecentrum gebruikt, wordt met **DLP-beleid** naar specifieke patronen en elementen ge zoekge gaan bij het detecteren van deze gevoelige typen.</span><span class="sxs-lookup"><span data-stu-id="e627a-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e627a-111">**Ingebouwde typen gevoelige informatie**</span><span class="sxs-lookup"><span data-stu-id="e627a-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e627a-112">Voor informatie over de ingebouwde typen gevoelige informatie en waar een DLP-beleid naar zoekt bij het detecteren van het type Gevoelig, gaat u naar: Waar wordt naar zoekt door de typen [gevoelige informatie.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e627a-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e627a-113">**Aangepaste typen gevoelige informatie**</span><span class="sxs-lookup"><span data-stu-id="e627a-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e627a-114">Als u aangepaste typen gevoelige informatie wilt maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast, gevoelig [type: Maak](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)een aangepast type gevoelige informatie.</span><span class="sxs-lookup"><span data-stu-id="e627a-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e627a-115">**Een DLP-beleid testen**</span><span class="sxs-lookup"><span data-stu-id="e627a-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e627a-116">Als u uw gegevens wilt testen met een ingebouwd of aangepast type gevoelige informatie, gebruikt u de optie **Testtype** onder   >  **Classificaties Gevoelige infotypen.**</span><span class="sxs-lookup"><span data-stu-id="e627a-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e627a-117">Zie Aangepaste typen gevoelige informatie [testen voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="e627a-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e627a-118">**Rapporten**</span><span class="sxs-lookup"><span data-stu-id="e627a-118">**Reports**</span></span>
  
- <span data-ttu-id="e627a-119">Krijg inzicht in gevoelige gegevens met [DLP-rapporten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e627a-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e627a-120">Specifieke details van de gebeurtenis bekijken met een [incidentenrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="e627a-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
