---
title: DLP-regel voor Us/UK Passport Number werkt niet
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004941"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP - US/UK-paspoortnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met amerikaanse/Britse paspoortnummers**

Hebt u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een Paspoortnummer van de **VS/VK** bevat bij het gebruik van een DLP-type gevoelige informatie in O365? Zo ja, zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een paspoortnummerbeleid van de **VS/VK** dat is geconfigureerd met een betrouwbaarheidsniveau van 75%, worden de volgende gegevens geëvalueerd en moet de regel worden gedetecteerd om de regel te activeren
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Negen cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Negen opeenvolgende cijfers

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Een DLP-beleid is 75% ervan overtuigd dat dit type gevoelige informatie is gedetecteerd als dit binnen een nabijheid van 300 tekens:

  - De functie Func_usa_uk_passport inhoud die overeenkomt met het patroon.

  - Er wordt een trefwoord Keyword_passport gevonden.

    In het volgende voorbeeld wordt bijvoorbeeld het paspoortnummerbeleid van de **VS/VK** in gang 123456789

Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is voor het detecteren van een Paspoortnummer voor de VS/VK voor uw inhoud: Wat de typen gevoelige informatie voor [us/UK Passport Number zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: Waar de typen gevoelige informatie naar zoeken met behulp van een ander ingebouwde [gevoelige informatietype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  