---
title: 'hetzelfde als de bestandsnaam is de beste [regel #-beschrijving]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697125"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="85854-102">Vereist Alchemie kop H1, H2 van werken niet.</span><span class="sxs-lookup"><span data-stu-id="85854-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="85854-103">Aanbevelingen en richtlijnen voor het ontwerpen van Alchemy:</span><span class="sxs-lookup"><span data-stu-id="85854-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="85854-p101">**Alchemy inzichten in mappen sluiten niet op elkaar**- dit, de url-structuur worden verbroken. We zijn op zoek naar deze vaststelling.</span><span class="sxs-lookup"><span data-stu-id="85854-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="85854-106">Bestanden in de map **AlchemyInsights** heeft regel-ID en de naam van de regel van de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) in de bestandsnaam.</span><span class="sxs-lookup"><span data-stu-id="85854-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="85854-p102">bijvoorbeeld ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="85854-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="85854-p103">De metagegevens aan de bovenkant van dit bestand gebruiken als uw sjabloon. Niets is vereist.</span><span class="sxs-lookup"><span data-stu-id="85854-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="85854-111">Ga naar de sectie in de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) **klant inzicht titel:** en gebruik die als een startpunt voor uw H1 titel voor het inzicht.</span><span class="sxs-lookup"><span data-stu-id="85854-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="85854-p104">Alchemy inzichten moet alleen een enkele H1 boven of ze in de productie worden verbroken. H2s weergeven niet in dat geval gebruik **vet** of andere overeenkomsten om aparte secties aan te geven.</span><span class="sxs-lookup"><span data-stu-id="85854-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="85854-114">Vul vervolgens de platte tekst met behulp van het materiaal van het concept in de sectie Customer Insights van de pagina regel Alchemy</span><span class="sxs-lookup"><span data-stu-id="85854-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="85854-115">Lijsten met opsommingstekens zijn fijn</span><span class="sxs-lookup"><span data-stu-id="85854-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="85854-116">Genummerde lijsten te</span><span class="sxs-lookup"><span data-stu-id="85854-116">Numbered lists too</span></span>
    1. <span data-ttu-id="85854-117">**Vet** en *cursief* zijn a-ok</span><span class="sxs-lookup"><span data-stu-id="85854-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="85854-118">Koppelingen moet altijd een **'koppelingen naar webpagina' / externe** of **diep-koppelingen naar de elementen van de gebruikersinterface**, geen interne koppelingen.</span><span class="sxs-lookup"><span data-stu-id="85854-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="85854-p105">En dit is echt al een beetje te lang. Beste is ongeveer 400 tekens---</span><span class="sxs-lookup"><span data-stu-id="85854-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="85854-p106">Zodra de inhoud gereed is, voeg alles aan levende tak. Vervolgens gaat u naar de [Alchemie Partner portal](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het veld url. Zorg ervoor dat inzicht gecontroleerd en gepubliceerd zegt "Ja" en klik op regel voor het bijwerken. **(Dit ziet er fraaier te verpakken in de nieuwe versie van de portal - spoedig vrijgeven.)** 
 ![url-veld](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="85854-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

