---
title: Aanmelden teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357551"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Aanmelden teams AADSTS9000411

Wanneer u zich aanmeldt bij Microsoft Teams, ontvangt u mogelijk de fout: **Sorry, maar we hebben problemen met het ondertekenen van u in AADSTS9000411: Het verzoek is niet goed opgemaakt. De parameter "login_hint" wordt gedupliceerd.**

Als u dit probleem wilt oplossen, moet u ervoor zorgen dat uw Microsoft Teams-clients worden bijgewerkt. Zie [Microsoft Teams bijwerken](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)voor meer informatie over het bijwerken van uw client.

Als u uw client om de een of andere reden niet bijwerken, worden de meeste gegevens in de cache gewist. Als u echter nog steeds problemen hebt na het afmelden/aanmelden, sluit u Teams en schakelt u de cache van uw client uit door het volgende te doen:
1. Sluit Microsoft Teams.
2. Ga naar: %appdata%\microsoft\teams en verwijder alle bestanden.
3. Microsoft Teams opnieuw openen.
