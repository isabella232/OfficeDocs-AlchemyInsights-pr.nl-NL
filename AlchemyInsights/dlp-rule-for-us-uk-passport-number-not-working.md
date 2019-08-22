---
title: DLP-regel voor de Verenigde Staten / Verenigd Koninkrijk paspoortnummer werkt niet
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
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529914"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemen met DLP - US / UK Passport getallen

Hebt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud die een **VS / VK paspoortnummer** wanneer u een type DLP gevoelige informatie in O365? Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor wat het DLP-beleid is op zoek naar wanneer deze wordt geëvalueerd.
  
Bijvoorbeeld voor een **VS / VK paspoortnummer** beleid is geconfigureerd met een betrouwbaarheidsniveau van 75%, de volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren
  
- **[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Negen cijfers

- **[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Negen opeenvolgende cijfers

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen controlesom

- **[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Een DLP-beleid is 75% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:

  - De functie Func_usa_uk_passport wordt gezocht naar inhoud die overeenkomt met het patroon.

  - Een sleutelwoord Keyword_passport is gevonden.

    Zoals in het volgende voorbeeld wordt voor de **VS / VK paspoortnummer** beleid: Amerikaans paspoort getal 123456789

Voor meer informatie over wat nodig voor een Amerikaanse is / paspoortnummer UK waargenomen voor uw inhoud, Zie de volgende sectie in dit artikel: [Wat de gevoelige soorten informatie uiterlijk voor Amerikaanse / paspoortnummer UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  