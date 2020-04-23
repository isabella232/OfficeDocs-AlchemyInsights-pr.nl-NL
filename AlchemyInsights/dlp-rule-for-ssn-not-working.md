---
title: DLP-regel voor SSN werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788697"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemen met sofinummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met SSN's**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **SSN (Social Security Number)** bevat bij het gebruik van een gevoelig informatietype in Microsoft 365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt. 
  
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
  