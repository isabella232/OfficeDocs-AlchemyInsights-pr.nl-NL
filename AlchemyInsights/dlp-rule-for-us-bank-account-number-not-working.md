---
title: DLP-regel voor bankrekeningnummer VS werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507329"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemen met bankrekeningnummers vs

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met bankrekeningnummers vs**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **Amerikaans bankrekeningnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een beleid voor **een Amerikaans bankrekeningnummer** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 opeenvolgende cijfers.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Een DLP-beleid is er 75% van overtuigd dat dit soort gevoelige informatie wordt gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De reguliere expressie Regex_usa_bank_account_number vindt inhoud die overeenkomt met het patroon

  - Er wordt een trefwoord uit Keyword_usa_Bank_Account gevonden.

    De volgende steekproef wordt bijvoorbeeld geactiveerd voor het beleid voor **bankrekeningnummer van** de VS: Betaalrekening 78344011

Zie het volgende gedeelte in dit artikel voor meer informatie over wat er nodig is om een **Amerikaans bankrekeningnummer** te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar bankrekeningnummer van de VS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Zie het volgende artikel met behulp van een ander ingebouwd type gevoelige informatie voor informatie over wat nodig is voor andere typen: [Waar de typen gevoelige informatie naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  