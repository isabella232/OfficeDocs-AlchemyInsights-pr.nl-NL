---
title: Adressering Teams aanmeldingsfout AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953010"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adressering Teams aanmeldingsfout AADSTS9000411

Wanneer u zich aanmeldt bij Microsoft Teams, krijgt u mogelijk de foutmelding: Sorry, maar we hebben problemen met het aanmelden **bij AADSTS9000411: De aanvraag is niet correct opgemaakt. De parameter 'login_hint' wordt gedupliceerd.**

Als u dit probleem wilt oplossen, moet u ervoor zorgen dat uw Microsoft Teams worden bijgewerkt. Zie Uw client bijwerken voor meer informatie over het bijwerken [van Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Als u uw client om wat voor reden dan ook niet kunt bijwerken, worden de meeste gegevens in de cache verwijderd als u zich afmeldt bij de client. Als u echter nog steeds problemen hebt na het logoff/aanmelding, sluit u de Teams en leegt u de clientcache door het volgende te doen:
1. Sluit Microsoft Teams.
2. Ga naar: %appdata%\microsoft\teams en verwijder alle bestanden.
3. Open Microsoft Teams.
