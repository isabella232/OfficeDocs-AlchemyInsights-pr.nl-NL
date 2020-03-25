---
title: DLP-regel voor creditcardnummer werkt niet
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932438"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemen met creditcardnummers

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

**DLP problemen met creditcardnummers**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **creditcardnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365? Zorg er zo voor dat uw inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer deze wordt geëvalueerd. Voor een **creditcardbeleid** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:
  
- **[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cijfers die kunnen worden opgemaakt of niet-geformatteerd (ddddddddddddddd) en moet de Luhn-test doorstaan.

- **[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zeer complex en robuust patroon dat kaarten van alle grote merken wereldwijd detecteert, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en dinerkaarten.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, de Luhn checksum

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De functie Func_credit_card vindt inhoud die overeenkomt met het patroon.

  - Een van de volgende is waar:

  - Er wordt een zoekwoord uit Keyword_cc_verification gevonden.

  - Er wordt een trefwoord uit Keyword_cc_name gevonden

  - De functie Func_expiration_date vindt een datum in de juiste datumnotatie.

  - De checksum passeert

    De volgende steekproef wordt bijvoorbeeld geactiveerd voor een DLP-creditcardnummerbeleid:

  - Visum: 4485 3647 3952 7352
  
  - Verloopt: 2/2009

Zie het volgende gedeelte in dit artikel voor meer informatie over wat er nodig is om een **creditcardnummer** voor uw inhoud te detecteren: [Wat de gevoelige informatietypen zoeken voor creditcardnummer#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  