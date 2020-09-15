---
title: DLP-regel voor creditcardnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679436"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemen met creditcardnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met creditcardnummers**

Ondervindt u problemen met **preventie van gegevensverlies (DLP)** voor inhoud met een **creditcardnummer** wanneer u een DLP gevoelige informatietype in O365 gebruikt? Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer het wordt geëvalueerd. Als u bijvoorbeeld een **creditcard beleid** hebt geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cijfers die wel of niet zijn opgemaakt (dddddddddddddddd) en de Luhn-test moeten doorlopen.

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zeer complex en krachtig patroon voor het detecteren van kaarten van alle belangrijkste merken wereldwijd, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeau kaarten en diner's cards.

- **[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, de Luhn-controlesom

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Een DLP-beleid is 85% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:

  - Met de functie Func_credit_card vindt u de inhoud die overeenkomt met het patroon.

  - Een van de volgende beweringen is waar:

  - Er is een trefwoord uit Keyword_cc_verification gevonden.

  - Een trefwoord uit Keyword_cc_name wordt gevonden

  - Met de functie Func_expiration_date vindt u een datum in de juiste datumnotatie.

  - De checksum verstuurt

    Met het volgende voorbeeld wordt bijvoorbeeld het beleid voor DLP-creditcardnummers geactiveerd:

  - Visa: 4485 3647 3952 7352
  
  - Verloopt over: 2/2009

Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor een **creditcardnummer** ter detectie van uw inhoud: [wat voor soort gevoelige informatie wordt weergegeven op een creditcard #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?
  