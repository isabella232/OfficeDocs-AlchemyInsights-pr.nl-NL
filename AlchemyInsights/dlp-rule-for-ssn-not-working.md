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
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507365"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemen met sofi-nummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met SSN's**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **Sofi-nummer (SSN)** bevat bij het gebruik van een gevoelig informatietype in Microsoft 365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid eruit ziet. 
  
Voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cijfers, die zich kunnen in een geformatteerd of niet-opgemaakt patroon hebben

- **[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar SSN's in vier verschillende patronen:

  - Func_ssn vindt SSN's met voor 2011 sterke opmaak die zijn opgemaakt met streepjes of spaties (ddd-dddd OF ddd ddd ddd dddd)

  - Func_unformatted_ssn vindt SSN's met een sterke opmaak vóór 2011 die niet zijn geformatteerd als negen opeenvolgende cijfers (dddddddddd)

  - Func_randomized_formatted_ssn vindt na 2011 SSN's die zijn opgemaakt met streepjes of spaties (ddd-dddd OF ddd ddd ddd dddd)

  - Func_randomized_unformatted_ssn vindt na 2011 SSNs die niet zijn geformatteerd als negen opeenvolgende cijfers (dddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat dit soort gevoelige informatie wordt gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De [functie Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) vindt inhoud die overeenkomt met het patroon.

  - Er wordt een trefwoord uit [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) gevonden. Voorbeelden van zoekwoorden zijn: *Sociale Zekerheid, Sociale Zekerheid#, Soc Sec, SSN* . De volgende steekproef wordt bijvoorbeeld geactiveerd voor het DLP SSN-beleid: **SSN: 489-36-8350**
  
Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om SSN's te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar SSN's](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Zie het volgende artikel met behulp van een ander ingebouwd type gevoelige informatie voor informatie over wat nodig is voor andere typen: [Waar de typen gevoelige informatie naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  