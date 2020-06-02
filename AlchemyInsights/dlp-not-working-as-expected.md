---
title: DLP werkt niet zoals verwacht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507473"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="42577-102">DLP werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="42577-102">DLP not working as expected</span></span>

<span data-ttu-id="42577-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="42577-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="42577-104">**DLP instellen**</span><span class="sxs-lookup"><span data-stu-id="42577-104">**Setting up DLP**</span></span>

<span data-ttu-id="42577-105">Heeft u problemen met **De Preventie van het Verlies van gegevens (DLP)** in Bureau 365 werkt niet zoals verwacht?</span><span class="sxs-lookup"><span data-stu-id="42577-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="42577-106">Zorg er dan voor dat uw **DLP-beleid** correct is ingesteld en dat uw gegevens bevatten wat het **DLP-beleid** zoekt wanneer deze worden geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="42577-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="42577-107">Met DLP-beleid u gevoelige informatie in uw organisatie identificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="42577-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="42577-108">Als u DLP-beleid wilt instellen, gebruikt u de informatie [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="42577-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="42577-109">**Wat DLP-beleid zoekt**</span><span class="sxs-lookup"><span data-stu-id="42577-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="42577-110">Wanneer u de **ingebouwde gevoelige informatietypen in** de beveiligings- en nalevingscentra gebruikt, zoekt DLP-beleid naar specifieke patronen en elementen bij het detecteren van deze gevoelige typen.</span><span class="sxs-lookup"><span data-stu-id="42577-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="42577-111">**Ingebouwde gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="42577-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="42577-112">Zie: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)voor informatie over de ingebouwde gevoelige typen en waar een DLP-beleid naar zoekt bij het detecteren van het gevoelige type.</span><span class="sxs-lookup"><span data-stu-id="42577-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="42577-113">**Aangepaste gevoelige informatietypen**</span><span class="sxs-lookup"><span data-stu-id="42577-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="42577-114">Als u aangepaste gevoelige informatietypen probeert te maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast gevoelig type: [Een aangepast gevoelig informatietype maken.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="42577-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="42577-115">**Een DLP-beleid testen**</span><span class="sxs-lookup"><span data-stu-id="42577-115">**Test a DLP policy**</span></span>

<span data-ttu-id="42577-116">Als u uw gegevens wilt testen met een ingebouwd of aangepast gevoelig informatietype, gebruikt u de optie **Type testen** onder **Classificaties**  >  **Gevoelige infotypen**.</span><span class="sxs-lookup"><span data-stu-id="42577-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="42577-117">Zie [Aangepaste gevoelige informatietypen testen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="42577-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="42577-118">**Rapporten**</span><span class="sxs-lookup"><span data-stu-id="42577-118">**Reports**</span></span>
  
- <span data-ttu-id="42577-119">Krijg gevoelige gegevensinzichten met [DLP-rapporten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="42577-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="42577-120">Zie specifieke details van het evenement met een [incidentrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="42577-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
