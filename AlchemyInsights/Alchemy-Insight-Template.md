---
title: hetzelfde als de bestandsnaam is het beste
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664129"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="92537-102">U kunt geen Alchemy-koptekst H1, H2's werkt niet. "</span><span class="sxs-lookup"><span data-stu-id="92537-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="92537-103">Aanbevolen procedures en richtlijnen voor het ontwerpen van Alchemy:</span><span class="sxs-lookup"><span data-stu-id="92537-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="92537-104">**Alchemy inzichten niet nesten in mappen**-Hiermee wordt de URL-structuur verbroken.</span><span class="sxs-lookup"><span data-stu-id="92537-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="92537-105">We zijn bezig dit te doen.</span><span class="sxs-lookup"><span data-stu-id="92537-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="92537-106">Bestanden in de **AlchemyInsights** -map moeten kleine letters bevatten met streepjes voor spaties ex.</span><span class="sxs-lookup"><span data-stu-id="92537-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="92537-107">in-en uitchecken van een ***zaak***.</span><span class="sxs-lookup"><span data-stu-id="92537-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="92537-108">Neem de regel-ID of de Bucket-ID op van de [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) in het veld MS. custom.</span><span class="sxs-lookup"><span data-stu-id="92537-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="92537-109">".</span><span class="sxs-lookup"><span data-stu-id="92537-109">ex.</span></span> <span data-ttu-id="92537-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="92537-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="92537-111">Gebruik de rest van de metagegevens aan het begin van dit bestand als uw sjabloon.</span><span class="sxs-lookup"><span data-stu-id="92537-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="92537-112">Ga in de [Partner Portal van Alchemy](https://alchemyportal.azurewebsites.net)naar de sectie met de **klant inzichten:** en gebruik dit als uitgangspunt voor de naam H1 voor de inzichten.</span><span class="sxs-lookup"><span data-stu-id="92537-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="92537-113">Alchemy Insights mag maar één van de andere H1-producten bevatten.</span><span class="sxs-lookup"><span data-stu-id="92537-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="92537-114">H2s wordt niet weergegeven, dus gebruik **vetgedrukte** of andere conventies om afzonderlijke secties aan te geven.</span><span class="sxs-lookup"><span data-stu-id="92537-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="92537-115">Vul vervolgens de hoofdtekst in met het concept materiaal in de sectie Customer inzichten van de pagina Alchemy regel</span><span class="sxs-lookup"><span data-stu-id="92537-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="92537-116">Lijsten met opsommingstekens zijn prima</span><span class="sxs-lookup"><span data-stu-id="92537-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="92537-117">Ook genummerde lijsten</span><span class="sxs-lookup"><span data-stu-id="92537-117">Numbered lists too</span></span>
    1. <span data-ttu-id="92537-118">**Vet** en *cursief* zijn een-OK</span><span class="sxs-lookup"><span data-stu-id="92537-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="92537-119">Koppelingen moeten altijd **' koppelingen naar web '/External** of **uitgebreide koppelingen naar gebruikersinterface-elementen**, geen interne koppelingen, zijn.</span><span class="sxs-lookup"><span data-stu-id="92537-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="92537-120">Afbeeldingen worden op dit moment niet ondersteund, maar het is in de routekaart.</span><span class="sxs-lookup"><span data-stu-id="92537-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="92537-121">Dit is eigenlijk al te lang.</span><span class="sxs-lookup"><span data-stu-id="92537-121">And this is really already a bit too long.</span></span> <span data-ttu-id="92537-122">Aanbevolen procedures voor 400-tekens---------------------------------</span><span class="sxs-lookup"><span data-stu-id="92537-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="92537-123">Als uw inhoud klaar is, trekt u deze naar de Live Branch.</span><span class="sxs-lookup"><span data-stu-id="92537-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="92537-124">Ga vervolgens naar de [Partner Portal van Alchemy](https://alchemyportal.azurewebsites.net) en typ de bestandsnaam in het veld URL.</span><span class="sxs-lookup"><span data-stu-id="92537-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 