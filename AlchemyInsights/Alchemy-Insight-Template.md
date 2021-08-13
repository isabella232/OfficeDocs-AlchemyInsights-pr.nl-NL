---
title: hetzelfde als bestandsnaam het beste is
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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918890"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>'Vereist Alchemy Header H1, H2's werken niet.'
Best Practices and guidelines for Alchemy authoring:

1. **Nest Alchemy-Insights niet in mappen.** Hierdoor wordt de url-structuur niet meer weergegeven. We zijn op zoek naar een oplossing.
1. Bestanden in **de map AlchemyInsights** moeten kleine letters bevatten met afbreekstreepen voor spaties ex. **_how-to-enable-litigation-hold_**.
    1. Neem de regel-id of bucket-id op van de [Portal alchemy-partner](https://alchemyportal.azurewebsites.net) in het veld ms.custom. ex. ***ms.custom: 100021***
1. Gebruik de rest van de metagegevens boven aan dit bestand als sjabloon.
1. [Navigeer in de portal Alchemy Partner](https://alchemyportal.azurewebsites.net)naar de sectie Customer Insight **Title:** en gebruik deze als uitgangspunt voor uw H1-titel voor het inzicht. 
    > [!NOTE]
    > Alchemy Insights moet slechts één H1 bovenaan hebben of ze breken in de productie. H2's worden niet weergegeven, dus gebruik **vet** of andere conventies om afzonderlijke secties aan te geven.
1. Vul vervolgens de hoofdtekst in met behulp van het conceptmateriaal in Customer Insights sectie van de pagina Alchemy-regel
    1. Lijsten met opsommingstekens zijn prima
    1. Genummerde lijsten ook
    1. **Vet** en *italisch* zijn a-ok
    1. Koppelingen moeten altijd **'koppelingen naar web' /externe** of **deep-links naar ui-elementen** zijn, niet interne koppelingen.
    1. Afbeeldingen worden momenteel niet officieel ondersteund, maar staan wel op de routekaart.

En dit is eigenlijk al iets te lang. Best practice is ongeveer 400 tekens ---------------------------------

Wanneer de inhoud gereed is, trekt u deze naar de live branch. Ga vervolgens naar de [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het url-veld in. 