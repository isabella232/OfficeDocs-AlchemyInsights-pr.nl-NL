---
title: DLP-regel voor US/UK-paspoortnummer werkt niet
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679219"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP-US/UK-paspoort nummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met US/UK-paspoort nummers**

Hebt u problemen met **preventie van preventie van gegevensverlies (DLP)** voor inhoud met een **US/UK-paspoortnummer** wanneer u een DLP gevoelige informatietype in O365 gebruikt? Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor de manier waarop het DLP-beleid zoekt wanneer het wordt geëvalueerd.
  
Als u bijvoorbeeld een beleid voor **US/UK Passport** hebt geconfigureerd met een betrouwbaarheidsniveau van 75%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel.
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Negen cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Negen opeenvolgende cijfers

- **[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen controlesom.

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Een DLP-beleid is 75% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:

  - Met de functie Func_usa_uk_passport vindt u de inhoud die overeenkomt met het patroon.

  - Er is een trefwoord uit Keyword_passport gevonden.

    Het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor het beleid voor **US/UK Passport** : US Passport Number 123456789

Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor een US/UK-paspoortnummer voor uw inhoud: [wat voor soort gevoelige informatie wordt gezocht naar het paspoortnummer van ons/VK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?
  