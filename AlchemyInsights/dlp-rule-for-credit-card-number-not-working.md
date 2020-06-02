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
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507401"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemen met creditcardnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met creditcardnummers**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **creditcardnummer** bevat bij het gebruik van een DLP-gevoelige informatietype in O365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer deze wordt geëvalueerd. Voor een **creditcardbeleid** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moeten worden gedetecteerd om de regel te activeren:
  
- **[Formaat:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cijfers die kunnen worden geformatteerd of niet-geformatteerd (ddddddddddddddddd) en moet de Luhn-test doorstaan.

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zeer complex en robuust patroon dat kaarten van alle grote merken wereldwijd detecteert, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en dinerkaarten.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, de Luhn checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat dit soort gevoelige informatie wordt gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De functie Func_credit_card vindt inhoud die overeenkomt met het patroon.

  - Een van de volgende is waar:

  - Er wordt een trefwoord uit Keyword_cc_verification gevonden.

  - Er wordt een trefwoord uit Keyword_cc_name gevonden

  - De functie Func_expiration_date vindt een datum in de juiste datumnotatie.

  - De checksum passeert

    De volgende steekproef wordt bijvoorbeeld geactiveerd voor een DLP-creditcardnummerbeleid:

  - Visum: 4485 3647 3952 7352
  
  - Afloopt: 2/2009

Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om een **creditcardnummer** te detecteren voor uw inhoud: [Wat de typen gevoelige informatie zoeken naar creditcardnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Zie het volgende artikel met behulp van een ander ingebouwd type gevoelige informatie voor informatie over wat nodig is voor andere typen: [Waar de typen gevoelige informatie naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  