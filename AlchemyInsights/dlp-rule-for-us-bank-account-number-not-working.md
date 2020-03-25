---
title: DLP-regel voor Amerikaans bankrekeningnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932524"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemen met Amerikaanse bankrekeningnummers

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

**DLP-problemen met Amerikaanse bankrekeningnummers**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **Amerikaans bankrekeningnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een beleid van **amerikaanse bankrekeningnummers** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:
  
- **[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cijfers

- **[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 opeenvolgende cijfers.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Een DLP-beleid is 75% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De reguliere expressie Regex_usa_bank_account_number vindt inhoud die overeenkomt met het patroon

  - Er wordt een trefwoord van Keyword_usa_Bank_Account gevonden.

    De volgende steekproef wordt bijvoorbeeld geactiveerd voor het beleid van het **Amerikaanse bankrekeningnummer:** Betaalrekening 78344011

Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om een **Amerikaans bankrekeningnummer** te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken voor het amerikaanse bankrekeningnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  