---
title: hetzelfde als bestandsnaam is het beste
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800040"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="98849-102">Vereiste Alchemy-header H1, H2's niet werken.</span><span class="sxs-lookup"><span data-stu-id="98849-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="98849-103">Best practices en richtlijnen voor het ontwerpen van Alchemy:</span><span class="sxs-lookup"><span data-stu-id="98849-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="98849-104">**Nest Alchemy Insights in mappen niet nesten**-hierdoor wordt de URL-structuur verbroken.</span><span class="sxs-lookup"><span data-stu-id="98849-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="98849-105">We zijn op zoek naar de vaststelling van dit.</span><span class="sxs-lookup"><span data-stu-id="98849-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="98849-106">Bestanden in de map **Alchemyinsights** moeten kleine bestandsnamen met afbreekstreepjes voor spaties ex hebben.</span><span class="sxs-lookup"><span data-stu-id="98849-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="98849-107">***Hoe te activeren-Litigation-Hold***.</span><span class="sxs-lookup"><span data-stu-id="98849-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="98849-108">Neem de regel-ID of Bucket-ID op uit de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in het veld MS. custom.</span><span class="sxs-lookup"><span data-stu-id="98849-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="98849-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="98849-109">ex.</span></span> <span data-ttu-id="98849-110">***MS. aangepast: 100021***</span><span class="sxs-lookup"><span data-stu-id="98849-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="98849-111">Gebruik de rest van de metagegevens boven aan dit bestand als sjabloon.</span><span class="sxs-lookup"><span data-stu-id="98849-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="98849-112">Navigeer in de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)naar de sectie **Customer Insight-Titel:** en gebruik dat als uitgangspunt voor uw H1-titel voor het inzicht.</span><span class="sxs-lookup"><span data-stu-id="98849-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="98849-113">Alchemy Insights moet slechts één H1 aan de bovenkant hebben of ze breken in de productie.</span><span class="sxs-lookup"><span data-stu-id="98849-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="98849-114">H2s niet renderen dus gebruik **vet** of andere conventies om afzonderlijke secties te duiden.</span><span class="sxs-lookup"><span data-stu-id="98849-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="98849-115">Vul vervolgens de hoofdtekst in met het concept materiaal in het gedeelte Customer Insights van de pagina Alchemy-regel</span><span class="sxs-lookup"><span data-stu-id="98849-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="98849-116">Lijsten met opsommingstekens zijn prima</span><span class="sxs-lookup"><span data-stu-id="98849-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="98849-117">Genummerde lijsten te</span><span class="sxs-lookup"><span data-stu-id="98849-117">Numbered lists too</span></span>
    1. <span data-ttu-id="98849-118">**Vet** en *cursief* zijn a-OK</span><span class="sxs-lookup"><span data-stu-id="98849-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="98849-119">Koppelingen moeten altijd zijn **' koppelingen naar web '/externe** of **Deep-links naar UI-elementen**, niet interne koppelingen.</span><span class="sxs-lookup"><span data-stu-id="98849-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="98849-120">Foto's worden op dit moment niet officieel ondersteund, maar het is op de roadmap.</span><span class="sxs-lookup"><span data-stu-id="98849-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="98849-121">En dit is echt al een beetje te lang.</span><span class="sxs-lookup"><span data-stu-id="98849-121">And this is really already a bit too long.</span></span> <span data-ttu-id="98849-122">Best Practice is ongeveer 400 tekens---------------------------------</span><span class="sxs-lookup"><span data-stu-id="98849-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="98849-123">Zodra uw inhoud klaar is, trekt u deze naar de Live-vertakking.</span><span class="sxs-lookup"><span data-stu-id="98849-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="98849-124">Ga vervolgens naar de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het URL-veld in.</span><span class="sxs-lookup"><span data-stu-id="98849-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 