---
title: DLP-regel voor het sofi-nummer niet werkt
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389428"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemen met sofi-nummers

Ondervindt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud met een **Sofi-nummer (Sofinummer)** bij gebruik van een type vertrouwelijke informatie in Office 365? Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor wat het DLP-beleid is op zoek. 
  
Bijvoorbeeld voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, het volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren:
  
- **[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cijfers bestaan, die mogelijk in een geformatteerde of ongeformatteerde patroon

- **[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken voor SSNs in vier verschillende patronen:

  - Func_ssn zoekt SSNs met pre-2011 sterke opmaak die zijn opgemaakt met streepjes of ruimten (ddd-dd-dddd of ddd dd dddd)

  - Func_unformatted_ssn zoekt SSNs met pre-2011 sterke opmaak die zijn geformatteerd als negen opeenvolgende cijfers (ddddddddd)

  - Func_randomized_formatted_ssn boeken-2011-SSNs die zijn opgemaakt met streepjes of ruimten (ddd-dd-dddd of ddd dd dddd) wordt gevonden

  - Func_randomized_unformatted_ssn zoekt boeken 2011-SSNs die geformatteerd als negen opeenvolgende cijfers (ddddddddd zijn)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nee, er is geen controlesom

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:

  - De [functie Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) wordt gezocht naar inhoud die overeenkomt met het patroon.

  - Een sleutelwoord [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is gevonden. Bevat voorbeelden van trefwoorden: *sociale zekerheid, sociale zekerheid #, Werknemerspremies, sofi-nummer* . Zoals in het volgende voorbeeld wordt voor de SSN DLP-beleid: **SSN: 489-36-8350**
  
Zie de volgende sectie in dit artikel voor meer informatie over wat is vereist voor SSNs voor uw inhoud worden gedetecteerd: [Wat de gevoelige soorten informatie zoekt SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  