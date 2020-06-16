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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750965"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Vereiste Alchemie Header H1, H2's werken niet."
Aanbevolen procedures en richtlijnen voor het schrijven van alchemie:

1. **Nest geen Alchemy Insights in mappen**- dit zal de url-structuur breken. We onderzoeken het repareren van dit.
1. Bestanden in de map **AlchemyInsights** moeten kleine bestandsnamen hebben met koppeltekens voor spaties ex. ***how-to-enable-litigation-hold***.
    1. Neem de regel-id of bucket-id op uit de [Alchemy Partner-portal](https://alchemyportal.azurewebsites.net) in het veld ms.custom. Ex. ***ms.custom: 100021***
1. Gebruik de rest van de metagegevens boven aan dit bestand als sjabloon.
1. Navigeer in de [Alchemy Partner-portal](https://alchemyportal.azurewebsites.net)naar de sectie **Customer Insight Title:** en gebruik die als uitgangspunt voor uw H1-titel voor het inzicht. 
    > [!NOTE]
    > Alchemie Insights MOET slechts een enkele H1 aan de top hebben of ze zullen breken in de productie. H2's maken geen gebruik van, dus gebruik **vet** of andere conventies om afzonderlijke secties aan te geven.
1. Vul vervolgens de hoofdtekst in met het conceptmateriaal in de sectie Customer Insights van de pagina Alchemieregel
    1. Lijsten met opsommingstekens zijn prima
    1. Ook genummerde lijsten
    1. **Vet** en *cursisch* zijn a-ok
    1. Links moeten altijd ofwel **"links naar web" / externe** of **deep-links naar UI-elementen,** niet interne links.
    1. Foto's worden op dit moment niet officieel ondersteund, maar het staat wel op de roadmap.

En dit is echt al een beetje te lang. Best practice is ongeveer 400 tekens ---------------------------------

Zodra uw inhoud klaar is, trekt u deze naar de live branch. Ga vervolgens naar de [Portal Alchemy Partner](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het url-veld in. 