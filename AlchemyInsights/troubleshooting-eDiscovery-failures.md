---
title: 1490-problemen oplossen-eDiscovery-fouten
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277841"
---
# <a name="troubleshoot-content-search-errors"></a>Problemen met zoeken in inhoud oplossen

Ondervindt u problemen met het zoeken van inhoud of het verkrijgen van fouten wanneer u zoekresultaten exporteert?

U ontvangt bijvoorbeeld het volgende wanneer u zoekopdrachten uitvoert?

- CS008-of CS012-fouten

- Beschikbaarheidsinfo Server-fouten

- Toepassingsfout opgetreden

Of bij het zoeken naar en exporteren van resultaten uit een groot aantal postvakken (meer dan 100.000 postvakken), krijgt u een exportfout?

Voor dit soort fouten probeert u het zoeken naar de inhoudslocaties die mislukt zijn. Zie  [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) voor meer informatie.

Als u meer dan een afgesloten 100k postvakken exporteert, moet u de volgende PowerShell gebruiken om de export resultaten te downloaden:  [resultaten uit meer dan afgesloten 100k postvakken exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
