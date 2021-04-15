---
title: 'Fout: De regels op deze computer komen niet overeen'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782947"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fout: De regels op deze computer komen niet overeen

Zie De regels op deze [computer](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) komen niet overeen met de regels op Microsoft Exchange als u de bijgewerkte status van dit bekende probleem wilt zien

Het Outlook-team heeft een oplossing geïmplementeerd in build 12928.10000. De oplossing is al bij Insider Fast en gaat eind juni 2020 naar Monthly Channel. Als u de vaste build hebt, krijgt u mogelijk nog één keer de vraag 'Welke regels wilt u behouden'. Kies Server wanneer u daarom wordt gevraagd en ga terug in Outlook en schakel alle uitgeschakelde regels opnieuw in.

Gebruik de volgende tijdelijke oplossing totdat de oplossing beschikbaar is:

**Tijdelijke oplossing:** In recente rapporten is het probleem opgetreden voor personen die alleen clientregels hebben gemaakt in de bureaubladversie van Outlook. Als u het probleem blijft tegen komen, kunt u overwegen de regels te verwijderen en vervolgens alleen regels te maken en te bewerken in OWA (Outlook Web App) totdat het probleem is opgelost.

Als u de regels niet handmatig kunt verwijderen, kunt u een Outlook-opdracht uitvoeren wanneer u Outlook start door Outlook.exe /cleanrules uit te voeren. Hiermee worden zowel de client- als de serverregels verwijderd. Hiermee worden alle regels voor alle accounts in het Outlook-profiel verwijderd. Deze opdracht wordt verder beschreven in het artikel Command-line switches.

