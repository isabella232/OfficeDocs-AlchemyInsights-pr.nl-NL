---
title: hetzelfde als bestandsnaam is het beste
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676528"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Vereist Alchemy Header H1, H2's werken niet.
Aanbevolen procedures en richtlijnen voor alchemie auteur:

1. **Nest Alchemy Insights niet in mappen**- dit zal de url-structuur breken. We onderzoeken of we dit willen oplossen.
1. Bestanden in de map **AlchemyInsights** moeten kleine bestandsnamen met koppeltekens hebben voor spaties, bijvoorbeeld. ***how-to-enable-litigation-hold***.
    1. Neem de regel-ID of bucket-ID op van de [Alchemy Partner-portal](https://alchemyportal.azurewebsites.net) in het veld ms.custom. Ex. ***ms.custom: 100021***
1. Gebruik de rest van de metagegevens boven aan dit bestand als sjabloon.
1. Navigeer in de [Portal van Alchemy Partner](https://alchemyportal.azurewebsites.net)naar de sectie Customer Insight **Title:** en gebruik dat als uitgangspunt voor uw H1-titel voor het inzicht. 
    > [!NOTE]
    > Alchemy Insights MOET slechts een enkele H1 aan de top of ze zullen breken in de productie. H2's maken niet renderen, dus gebruik **vet** of andere conventies om afzonderlijke secties aan te duiden.
1. Vul vervolgens de hoofdtekst in met het conceptmateriaal in de sectie Customer Insights van de pagina Alchemieregel
    1. Lijsten met opsommingstekens zijn prima
    1. Genummerde lijsten ook
    1. **Vet** en *cursief* zijn a-ok
    1. Links moeten altijd ofwel **"links naar web"/ externe** of **deep-links naar UI-elementen,** geen interne links.
    1. Foto's worden op dit moment niet officieel ondersteund, maar het staat wel op de roadmap.

En dit is echt al een beetje te lang. Best practice is ongeveer 400 tekens ---------------------------------

Zodra uw inhoud klaar is, trekt u deze naar de live-branch. Ga vervolgens naar de [Alchemy Partner-portal](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het url-veld in. 