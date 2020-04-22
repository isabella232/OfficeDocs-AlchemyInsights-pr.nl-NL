---
title: DLP-regel voor creditcardnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704196"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemen met creditcardnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

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
  