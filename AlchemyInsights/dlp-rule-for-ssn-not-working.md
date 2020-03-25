---
title: DLP-regel voor SSN werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932516"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemen met sofinummers

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

**DLP-problemen met SSN's**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **SSN (Social Security Number)** bevat bij het gebruik van een gevoelig informatietype in Office 365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt. 
  
Voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:
  
- **[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cijfers, die zich in een opgemaakt of niet-opgemaakt patroon kunnen begeven

- **[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar SSN's in vier verschillende patronen:

  - Func_ssn vindt SSN's met een sterke opmaak van voor 2011 die zijn opgemaakt met streepjes of spaties (ddd-dddd of ddd dddd)

  - Func_unformatted_ssn vindt SSN's met een sterke opmaak van voor 2011 die niet zijn opgemaakt als negen opeenvolgende cijfers (ddddddddd)

  - Func_randomized_formatted_ssn vindt ssn's na 2011 die zijn opgemaakt met streepjes of spaties (ddd-dddd of ddd dddd)

  - Func_randomized_unformatted_ssn vindt ssn na 2011 zonder opmaak als negen opeenvolgende cijfers (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De [functie Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) vindt inhoud die overeenkomt met het patroon.

  - Er wordt een trefwoord uit [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) gevonden. Voorbeelden van trefwoorden zijn: *Sociale Zekerheid, Sociale Zekerheid#, Soc Sec, SSN* . De volgende steekproef wordt bijvoorbeeld geactiveerd voor het DLP SSN-beleid: **SSN: 489-36-8350**
  
Zie het volgende gedeelte in dit artikel [voor](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn) meer informatie over wat er nodig is om SSN's te detecteren voor uw inhoud.
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  