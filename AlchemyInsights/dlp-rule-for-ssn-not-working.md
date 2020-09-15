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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679364"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemen met sofi-nummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met naar ssn's**

Ondervindt u problemen met **preventie van gegevensverlies (DLP)** voor inhoud met een **sofi-nummer (SSN)** voor het gebruik van een type gevoelige informatie in Microsoft 365? Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor het opzoeken van het DLP-beleid. 
  
Als u bijvoorbeeld een SSN-beleid hebt geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cijfers in een opgemaakt of niet-opgemaakt patroon

- **[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar naar ssn's met vier verschillende patronen:

  - Met Func_ssn vindt u naar ssn's met een sterke opmaak van vóór 2011, opgemaakt met streepjes of spaties (ddd-DD-dddd of ddd DD dddd)

  - Met Func_unformatted_ssn vindt u naar ssn's met een sterke opmaak van vóór 2011 die niet is opgemaakt als negen opeenvolgende cijfers (ddddddddd)

  - Met Func_randomized_formatted_ssn vindt u post-2011-naar ssn's die zijn opgemaakt met streepjes of spaties (ddd-DD-dddd of ddd DD dddd)

  - Met Func_randomized_unformatted_ssn vindt u post-2011-naar ssn's die niet zijn opgemaakt als negen opeenvolgende cijfers (ddddddddd)

- **[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nee, er is geen controlesom.

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Een DLP-beleid is 85% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:

  - Met de [functie Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) vindt u de inhoud die overeenkomt met het patroon.

  - Er is een trefwoord uit [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) gevonden. Voorbeelden van trefwoorden  *zijn: Social Security, Social Security #, SOC sec, SSN*  . Het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor het DLP-SSN-beleid: **SSN: 489-36-8350**
  
Zie de volgende sectie in dit artikel voor meer informatie over de vereisten voor naar ssn's voor uw inhoud: de [typen gevoelige informatie zoekt](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) u naar naar ssn's
  
Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?
  