---
title: Zelfde als filename is de beste
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
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366326"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fabe8-102">Vereist Alchemie kop H1, H2 van werken niet.</span><span class="sxs-lookup"><span data-stu-id="fabe8-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="fabe8-103">Aanbevelingen en richtlijnen voor het ontwerpen van Alchemy:</span><span class="sxs-lookup"><span data-stu-id="fabe8-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fabe8-104">**Alchemy inzichten in mappen sluiten niet op elkaar**- dit, de url-structuur worden verbroken.</span><span class="sxs-lookup"><span data-stu-id="fabe8-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fabe8-105">We zijn op zoek naar deze vaststelling.</span><span class="sxs-lookup"><span data-stu-id="fabe8-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fabe8-106">Bestanden in de map **AlchemyInsights** moeten in kleine letters bestandsnamen met afbreekstreepjes Spaces ex hebben.</span><span class="sxs-lookup"><span data-stu-id="fabe8-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fabe8-107">***how-naar-enable-rechtszaak-hold***.</span><span class="sxs-lookup"><span data-stu-id="fabe8-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fabe8-108">De regel-ID of bucket-ID van de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) in het veld ms.custom opnemen.</span><span class="sxs-lookup"><span data-stu-id="fabe8-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fabe8-109">ex.</span><span class="sxs-lookup"><span data-stu-id="fabe8-109">ex.</span></span> <span data-ttu-id="fabe8-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="fabe8-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fabe8-111">De rest van de metagegevens aan de bovenkant van dit bestand gebruiken als uw sjabloon.</span><span class="sxs-lookup"><span data-stu-id="fabe8-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fabe8-112">Ga naar de sectie in de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) **klant inzicht titel:** en gebruik die als een startpunt voor uw H1 titel voor het inzicht.</span><span class="sxs-lookup"><span data-stu-id="fabe8-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fabe8-113">Alchemy inzichten moet alleen een enkele H1 boven of ze in de productie worden verbroken.</span><span class="sxs-lookup"><span data-stu-id="fabe8-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fabe8-114">H2s weergeven niet in dat geval gebruik **vet** of andere overeenkomsten om aparte secties aan te geven.</span><span class="sxs-lookup"><span data-stu-id="fabe8-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fabe8-115">Vul vervolgens de platte tekst met behulp van het materiaal van het concept in de sectie Customer Insights van de pagina regel Alchemy</span><span class="sxs-lookup"><span data-stu-id="fabe8-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fabe8-116">Lijsten met opsommingstekens zijn fijn</span><span class="sxs-lookup"><span data-stu-id="fabe8-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fabe8-117">Genummerde lijsten te</span><span class="sxs-lookup"><span data-stu-id="fabe8-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fabe8-118">**Vet** en *cursief* zijn a-ok</span><span class="sxs-lookup"><span data-stu-id="fabe8-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fabe8-119">Koppelingen moet altijd een **'koppelingen naar webpagina' / externe** of **diep-koppelingen naar de elementen van de gebruikersinterface**, geen interne koppelingen.</span><span class="sxs-lookup"><span data-stu-id="fabe8-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fabe8-120">Afbeeldingen worden niet officieel ondersteund op dit moment, maar het is op de routekaart.</span><span class="sxs-lookup"><span data-stu-id="fabe8-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fabe8-121">En dit is echt al een beetje te lang.</span><span class="sxs-lookup"><span data-stu-id="fabe8-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fabe8-122">Beste is ongeveer 400 tekens---</span><span class="sxs-lookup"><span data-stu-id="fabe8-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fabe8-123">Zodra de inhoud gereed is, voeg alles aan levende tak.</span><span class="sxs-lookup"><span data-stu-id="fabe8-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fabe8-124">Vervolgens gaat u naar de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het veld url.</span><span class="sxs-lookup"><span data-stu-id="fabe8-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="fabe8-125">M</span><span class="sxs-lookup"><span data-stu-id="fabe8-125">M</span></span>