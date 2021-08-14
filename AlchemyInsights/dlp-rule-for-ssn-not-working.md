---
title: DLP-regel voor SSN werkt niet
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004977"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemen met sociale-zekerheidsnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met SSN's**

Hebt u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **SSN (Social Security Number)** bevat bij het gebruik van een type gevoelige informatie in Microsoft 365? Zo ja, zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt. 
  
Voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende gegevens geëvalueerd en moet de regel worden gedetecteerd om de regel te activeren:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cijfers, die mogelijk een opgemaakt of niet-opgemaakt patroon hebben

- **[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar SSN's in vier verschillende patronen:

  - Func_ssn vindt SSN's met een sterke opmaak van vóór 2011 die zijn opgemaakt met streepjes of spaties (ddd-ddddd OR ddd ddddd)

  - Func_unformatted_ssn vindt SSN's met een sterke opmaak van vóór 2011 die niet is opgemaakt als negen opeenvolgende cijfers (ddddddddd)

  - Func_randomized_formatted_ssn zoekt naar SSN's na 2011 die zijn opgemaakt met streepjes of spaties (ddd-dd-dddd OF ddd dd)

  - Func_randomized_unformatted_ssn wordt na 2011 SSN's gevonden die niet zijn opgemaakt als negen opeenvolgende cijfers (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat dit type gevoelige informatie is gedetecteerd als dit binnen een nabijheid van 300 tekens:

  - Met [de Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) wordt inhoud gevonden die overeenkomt met het patroon.

  - Er wordt een [trefwoord Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) gevonden. Voorbeelden van trefwoorden zijn:  *Sociale zekerheid, Sociale zekerheid#, Soc Sec , SSN*  . Het volgende voorbeeld zou bijvoorbeeld leiden tot het DLP SSN-beleid: **SSN: 489-36-8350**
  
Zie de volgende sectie in dit artikel: Wat de typen gevoelige informatie voor [SSN's](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) zoeken voor SSN's voor meer informatie over wat vereist is voor het detecteren van SSN's voor uw inhoud
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: Waar de typen gevoelige informatie naar zoeken met behulp van een ander ingebouwde [gevoelige informatietype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  