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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930128"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Best practices toepassen voor geavanceerde zoekquery's

Als u sneller resultaten wilt boeken en time-outs wilt vermijden tijdens het uitvoeren van complexe query's, past u de volgende best practices toe:

- Wanneer u nieuwe query's probeert, gebruikt u altijd een limiet om te voorkomen dat u zeer grote resultatensets krijgt. Gebruik deze optie ook om een eerste beoordeling te maken van de grootte van `count` de resultatenset.
- Gebruik eerst tijdfilters. Beperk uw query's in het ideale ideaal tot zeven dagen.
- Voeg aan het begin van een query, direct na het tijdfilter, de filters toe die naar verwachting de meeste gegevens zullen verwijderen.
- Wanneer u op zoek bent naar volledige tokens, gebruikt u de `has` operator in plaats van `contains` .
- Voer een zoekopdracht uit in een specifieke kolom in plaats van in alle kolommen.
- Geef bij het deelnemen aan tabellen eerst de tabel op met minder rijen.
- `project` alleen de benodigde kolommen uit de tabellen die u hebt samengevoegd.

Zie Geavanceerde best practices [voor query's voor query's voor geavanceerde query's voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144812)
