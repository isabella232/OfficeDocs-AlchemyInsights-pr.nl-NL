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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679688"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="0a09d-102">DLP werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="0a09d-102">DLP not working as expected</span></span>

<span data-ttu-id="0a09d-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0a09d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="0a09d-104">**DLP instellen**</span><span class="sxs-lookup"><span data-stu-id="0a09d-104">**Setting up DLP**</span></span>

<span data-ttu-id="0a09d-105">Hebt u problemen met **preventie van gegevensverlies (DLP)** in Office 365 werkt niet zoals verwacht?</span><span class="sxs-lookup"><span data-stu-id="0a09d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="0a09d-106">Zorg er daarom voor dat het **DLP-beleid** correct is ingesteld, en dat uw gegevens bevatten wat het **DLP-beleid** zocht wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="0a09d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="0a09d-107">DLP-beleid biedt u de mogelijkheid gevoelige informatie in uw organisatie te identificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="0a09d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="0a09d-108">Voor het instellen van DLP-beleidsregels gebruikt u de gegevens [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="0a09d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="0a09d-109">**Welk DLP-beleid zoekt**</span><span class="sxs-lookup"><span data-stu-id="0a09d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="0a09d-110">Wanneer u de **ingebouwde gevoelige informatie typen** in de beveiligings-en compliance Centers gebruikt, zoeken DLP-beleidsregels naar specifieke patronen en elementen wanneer deze gevoelige typen worden gedetecteerd.</span><span class="sxs-lookup"><span data-stu-id="0a09d-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="0a09d-111">**Ingebouwde gevoelige informatie typen**</span><span class="sxs-lookup"><span data-stu-id="0a09d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="0a09d-112">Zie voor meer informatie over de ingebouwde typen gevoelige typen en wat een DLP-beleid controleert wanneer u het gevoelige type opspoort, voor meer informatie: [hoe de typen gevoelige informatie eruitzien](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="0a09d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="0a09d-113">**Aangepaste gevoelige informatie typen**</span><span class="sxs-lookup"><span data-stu-id="0a09d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="0a09d-114">Als u aangepaste typen gevoelige informatie wilt maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast gevoelig type: [Maak een aangepast gevoelige informatietype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0a09d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="0a09d-115">**DLP-beleid testen**</span><span class="sxs-lookup"><span data-stu-id="0a09d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="0a09d-116">Als u uw gegevens wilt testen met een ingebouwd of aangepast type gevoelige informatie, gebruikt u de optie **testtype** onder **indelings**  >  **gevoelige info typen**.</span><span class="sxs-lookup"><span data-stu-id="0a09d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0a09d-117">Zie voor meer informatie [aangepaste, gevoelige informatie typen testen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="0a09d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="0a09d-118">**Rapporten**</span><span class="sxs-lookup"><span data-stu-id="0a09d-118">**Reports**</span></span>
  
- <span data-ttu-id="0a09d-119">U ontvangt gevoelige gegevens inzichten met [DLP-rapporten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="0a09d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="0a09d-120">Bepaalde details van het evenement bekijken met een [incident rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="0a09d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
