---
title: DLP-regel voor amerikaans/Brits paspoortnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507293"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP - Amerikaans/Britse paspoortnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP problemen met de VS / Uk paspoortnummers**

Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **Amerikaans/Brits paspoortnummer** bevat bij het gebruik van een DLP-gevoelige informatietype in O365? Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een **amerikaans/Brits paspoortnummerbeleid** dat is geconfigureerd met een betrouwbaarheidsniveau van 75%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd dat de regel kan worden geactiveerd
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Negen cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Negen opeenvolgende cijfers

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Een DLP-beleid is er 75% van overtuigd dat dit soort gevoelige informatie wordt gedetecteerd als, binnen een nabijheid van 300 tekens:

  - De functie Func_usa_uk_passport vindt inhoud die overeenkomt met het patroon.

  - Er wordt een trefwoord uit Keyword_passport gevonden.

    De volgende steekproef wordt bijvoorbeeld geactiveerd voor het beleid voor **paspoortnummer vs/UK:** U.S. Passport number 123456789

Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om een Amerikaans/Brits paspoortnummer te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar amerikaans/Brits paspoortnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Zie het volgende artikel met behulp van een ander ingebouwd type gevoelige informatie voor informatie over wat nodig is voor andere typen: [Waar de typen gevoelige informatie naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  