---
title: 'Fout: De regels op deze computer komen niet overeen'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664241"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fout: De regels op deze computer komen niet overeen

Zie De regels op deze [computer komen niet overeen met de regels voor Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Het Outlook-team heeft een oplossing geïmplementeerd in Build 12928.10000. De fix is al bij Insider Fast en zal eind juni 2020 naar Monthly Channel gaan. Zodra u de vaste build u de prompt Welke regels wil je houden een laatste keer. Kies Server wanneer daarom wordt gevraagd en ga vervolgens terug in Outlook en schakel alle uitgeschakelde regels opnieuw in.

Totdat de oplossing beschikbaar is, gebruikt u de volgende tijdelijke oplossing:

**Tijdelijke oplossing**: In recente rapporten is het probleem opgetreden voor degenen die alleen clientregels hebben gemaakt in Outlook-bureaublad. Als u het probleem blijft tegenkomen, u overwegen de regels te verwijderen en vervolgens alleen regels maken en bewerken in OWA (Outlook Web App) totdat het probleem is opgelost.

Als u de regels niet handmatig verwijderen, u een Outlook-opdracht uitvoeren wanneer u Outlook start door Outlook.exe /cleanrules uit te voeren. Hiermee worden zowel de client- als de serverregels verwijderd. Hiermee worden alle regels verwijderd voor alle accounts in het Outlook-profiel. Deze opdracht wordt verder gedocumenteerd in het artikel Command-line switches.

