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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800040"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Vereiste Alchemy-header H1, H2's niet werken.
Best practices en richtlijnen voor het ontwerpen van Alchemy:

1. **Nest Alchemy Insights in mappen niet nesten**-hierdoor wordt de URL-structuur verbroken. We zijn op zoek naar de vaststelling van dit.
1. Bestanden in de map **Alchemyinsights** moeten kleine bestandsnamen met afbreekstreepjes voor spaties ex hebben. ***Hoe te activeren-Litigation-Hold***.
    1. Neem de regel-ID of Bucket-ID op uit de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in het veld MS. custom. Ex. ***MS. aangepast: 100021***
1. Gebruik de rest van de metagegevens boven aan dit bestand als sjabloon.
1. Navigeer in de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)naar de sectie **Customer Insight-Titel:** en gebruik dat als uitgangspunt voor uw H1-titel voor het inzicht. 
    > [!NOTE]
    > Alchemy Insights moet slechts één H1 aan de bovenkant hebben of ze breken in de productie. H2s niet renderen dus gebruik **vet** of andere conventies om afzonderlijke secties te duiden.
1. Vul vervolgens de hoofdtekst in met het concept materiaal in het gedeelte Customer Insights van de pagina Alchemy-regel
    1. Lijsten met opsommingstekens zijn prima
    1. Genummerde lijsten te
    1. **Vet** en *cursief* zijn a-OK
    1. Koppelingen moeten altijd zijn **' koppelingen naar web '/externe** of **Deep-links naar UI-elementen**, niet interne koppelingen.
    1. Foto's worden op dit moment niet officieel ondersteund, maar het is op de roadmap.

En dit is echt al een beetje te lang. Best Practice is ongeveer 400 tekens---------------------------------

Zodra uw inhoud klaar is, trekt u deze naar de Live-vertakking. Ga vervolgens naar de [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) en voer de bestandsnaam in het URL-veld in. 