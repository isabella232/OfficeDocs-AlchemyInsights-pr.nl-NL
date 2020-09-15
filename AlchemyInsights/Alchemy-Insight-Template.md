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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>U kunt geen Alchemy-koptekst H1, H2's werkt niet. "
Aanbevolen procedures en richtlijnen voor het ontwerpen van Alchemy:

1. **Alchemy inzichten niet nesten in mappen**-Hiermee wordt de URL-structuur verbroken. We zijn bezig dit te doen.
1. Bestanden in de **AlchemyInsights** -map moeten kleine letters bevatten met streepjes voor spaties ex. in-en uitchecken van een ***zaak***.
    1. Neem de regel-ID of de Bucket-ID op van de [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) in het veld MS. custom. ". ***MS. Custom: 100021***
1. Gebruik de rest van de metagegevens aan het begin van dit bestand als uw sjabloon.
1. Ga in de [Partner Portal van Alchemy](https://alchemyportal.azurewebsites.net)naar de sectie met de **klant inzichten:** en gebruik dit als uitgangspunt voor de naam H1 voor de inzichten. 
    > [!NOTE]
    > Alchemy Insights mag maar één van de andere H1-producten bevatten. H2s wordt niet weergegeven, dus gebruik **vetgedrukte** of andere conventies om afzonderlijke secties aan te geven.
1. Vul vervolgens de hoofdtekst in met het concept materiaal in de sectie Customer inzichten van de pagina Alchemy regel
    1. Lijsten met opsommingstekens zijn prima
    1. Ook genummerde lijsten
    1. **Vet** en *cursief* zijn een-OK
    1. Koppelingen moeten altijd **' koppelingen naar web '/External** of **uitgebreide koppelingen naar gebruikersinterface-elementen**, geen interne koppelingen, zijn.
    1. Afbeeldingen worden op dit moment niet ondersteund, maar het is in de routekaart.

Dit is eigenlijk al te lang. Aanbevolen procedures voor 400-tekens---------------------------------

Als uw inhoud klaar is, trekt u deze naar de Live Branch. Ga vervolgens naar de [Partner Portal van Alchemy](https://alchemyportal.azurewebsites.net) en typ de bestandsnaam in het veld URL. 