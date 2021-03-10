---
title: Best practices toepassen voor geavanceerde zoekquery's
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693346"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Best practices toepassen voor geavanceerde zoekquery's

Als u sneller resultaten wilt krijgen en time-outs wilt vermijden tijdens het uitvoeren van complexe query's, moet u de volgende best practices toepassen:

- Wanneer u nieuwe query's probeert, moet u altijd een limiet gebruiken om te voorkomen dat u zeer grote resultatensets krijgt. Gebruik deze optie ook om een eerste evaluatie te maken van de grootte `count` van de resultatenset.
- Gebruik eerst tijdfilters. Beperk uw query's het beste tot zeven dagen.
- Aan het begin van een query, direct na het tijdfilter, voegt u de filters toe die de meeste gegevens naar verwachting zullen verwijderen.
- Als u op zoek bent naar volledige tokens, gebruikt u de `has` operator in plaats van `contains` .
- Voer een zoekopdracht uit op een specifieke kolom in plaats van voor alle kolommen.
- Wanneer u tabellen wilt samenvoegen, geeft u eerst de tabel met minder rijen op.
- `project` alleen de benodigde kolommen uit de tabellen die u hebt samengevoegd.

Zie geavanceerde [zoekquery-best practices voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144812)
