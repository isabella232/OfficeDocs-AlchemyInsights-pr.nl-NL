---
title: Aanmeldingsfout voor Teams aanpakken AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821982"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Aanmeldingsfout voor Teams aanpakken AADSTS9000411

Wanneer u zich aanmeldt bij Microsoft Teams, krijgt u mogelijk de foutmelding: Sorry, maar we hebben problemen met het ondertekenen van u **in AADSTS9000411: De aanvraag is niet correct opgemaakt. De parameter 'login_hint' wordt gedupliceerd.**

Als u dit probleem wilt oplossen, moet u ervoor zorgen dat uw Microsoft Teams-clients worden bijgewerkt. Zie Microsoft Teams bijwerken voor meer informatie over het bijwerken [van uw client.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Als u uw client om wat voor reden dan ook niet kunt bijwerken, worden de meeste gegevens in de cache verwijderd als u zich afmeldt bij de client. Als u echter nog steeds problemen hebt na het logoff/aanmelding, sluit u Teams af en leegt u de cache van uw client door het volgende te doen:
1. Sluit Microsoft Teams.
2. Ga naar: %appdata%\microsoft\teams en verwijder alle bestanden.
3. Open Microsoft Teams opnieuw.
