---
title: DLP-regel voor US Bank-account nummer werkt niet
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679291"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemen met US bankrekening nummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met US bankrekening nummers**

Hebt u problemen met **preventie van preventie van gegevensverlies (DLP)** voor inhoud met een **account van een Amerikaanse bank rekening** wanneer u een DLP gevoelige informatietype in O365 gebruikt? Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor de manier waarop het DLP-beleid zoekt wanneer het wordt geëvalueerd.
  
Voor het **account nummer van een US Bank** is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:
  
- **[Notatie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 opeenvolgende cijfers.

- **[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen controlesom.

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Een DLP-beleid is 75% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:

  - Met de reguliere expressie Regex_usa_bank_account_number u inhoud vindt die overeenkomt met het patroon.

  - Er is een trefwoord uit Keyword_usa_Bank_Account gevonden.

    Met het volgende voorbeeld wordt bijvoorbeeld het 78344011 beleid voor het **accountnummer** van uw account in de VS

Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor de inhoud van uw account in de **Verenigde Staten** : met [de typen gevoelige informatie wordt gezocht naar het accountnummer van de Amerikaanse bank](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .
  
Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?
  