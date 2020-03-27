---
title: DLP-regel voor paspoortnummer VS/VK werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977101"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP - Paspoortnummers VS/VK

**Belangrijk:** Tijdens deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services zeer beschikbaar blijven - Ga naar [tijdelijke functieaanpassingen van SharePoint Online](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP problemen met de VS / UK paspoortnummers**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **paspoortnummer tussen de VS en het VK** bevat bij het gebruik van een DLP-gevoelig informatietype in O365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een **paspoortnummerbeleid tussen de VS en het VK** dat is geconfigureerd met een betrouwbaarheidsniveau van 75%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd om de regel te activeren
  
- **[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Negen cijfers

- **[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Negen opeenvolgende cijfers

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Een DLP-beleid is 75% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De functie Func_usa_uk_passport vindt inhoud die overeenkomt met het patroon.

  - Er wordt een trefwoord uit Keyword_passport gevonden.

    De volgende steekproef zou bijvoorbeeld leiden tot het beleid van het paspoortnummer tussen de **VS en het Verenigd Koninkrijk:** Amerikaans paspoortnummer 123456789

Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om een paspoortnummer tussen de VS en het VK te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar het paspoortnummer tussen de VS en het Vk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  