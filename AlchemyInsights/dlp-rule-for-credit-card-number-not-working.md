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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005085"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemen met creditcardnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met creditcardnummers**

Hebt u problemen met **Data Loss Prevention (DLP)**  die niet werkt voor inhoud die een creditcardnummer bevat bij het gebruik van een DLP-gevoelige informatietype in O365? Zo ja, zorg er dan voor dat uw inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer deze wordt geëvalueerd. Voor een creditcardbeleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende gegevens geëvalueerd en moet de regel worden gedetecteerd om de regel te activeren: 
  
- **[Notatie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cijfers die kunnen worden opgemaakt of niet-opgemaakt (ddddd) en moeten de Luhn-toets doorstaan.

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zeer complex en robuust patroon dat kaarten van alle grote merken wereldwijd detecteert, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeaukaarten en dinerkaarten.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, de Luhn-checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat dit type gevoelige informatie is gedetecteerd als dit binnen een nabijheid van 300 tekens:

  - De functie Func_credit_card inhoud die overeenkomt met het patroon.

  - Een van de volgende gegevens is waar:

  - Er wordt een trefwoord Keyword_cc_verification gevonden.

  - Er wordt een trefwoord Keyword_cc_name gevonden

  - Met de Func_expiration_date wordt een datum in de juiste datumnotatie gevonden.

  - De checksum passeert

    In het volgende voorbeeld wordt bijvoorbeeld een DLP-creditcardnummerbeleid in gang gestaan:

  - Visa: 4485 3647 3952 7352
  
  - Verloopt: 2-2009

Zie de volgende sectie in  dit artikel voor meer informatie over wat nodig is voor het detecteren van een creditcardnummer voor uw inhoud: Wat de typen gevoelige informatie zoeken [voor Creditcard#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: Waar de typen gevoelige informatie naar zoeken met behulp van een ander ingebouwde [gevoelige informatietype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  