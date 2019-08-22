---
title: DLP-regel voor het nummer van de creditcard niet werkt
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529950"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemen met nummers van creditcards DLP

Ondervindt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud met een **Creditcardnummer** als u een type DLP gevoelige informatie in O365? Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor het starten van de het DLP-beleid als het wordt geëvalueerd. Bijvoorbeeld voor een **creditcard beleid** geconfigureerd met een betrouwbaarheidsniveau van 85%, het volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren:
  
- **[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cijfers nauwkeurig, hetgeen kunnen worden opgemaakt of niet-opgemaakte (dddddddddddddddd) en de test Luhn moet doorgeven.

- **[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Krachtige en zeer complex patroon dat kaarten van alle belangrijke merken over de hele wereld, met inbegrip van Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en diner kaarten detecteert.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, de controlesom Luhn

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:

  - De functie Func_credit_card wordt gezocht naar inhoud die overeenkomt met het patroon.

  - Het volgende geldt:

  - Een sleutelwoord Keyword_cc_verification is gevonden.

  - Een sleutelwoord Keyword_cc_name is gevonden.

  - De functie Func_expiration_date wordt een datum in de juiste notatie.

  - De controlesom wordt doorgegeven

    In het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor een beleid van DLP Credit Card nummer:

  - Visa: 4485 3647 3952 7352
  
  - Verloopt: 2-2009

Zie de volgende sectie in dit artikel voor meer informatie over wat nodig voor een **Creditcardnummer is** waargenomen voor uw inhoud: [Wat de gevoelige soorten informatie zoeken voor creditcard #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  