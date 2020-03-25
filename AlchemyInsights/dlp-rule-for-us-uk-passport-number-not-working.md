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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931257"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP - Paspoortnummers VS/VK

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

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
  