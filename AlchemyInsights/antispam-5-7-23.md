---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932164"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met e-mailbezorging oplossen voor foutcode 5.7.23

Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op het web.

Controleer of het uitgaande bericht niet is geïdentificeerd als spam door Microsoft en door de groep met hoge [risicobezorging is gerouteerd.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Berichten in de groep Bezorging met hoog risico worden niet door SPF-controles uitgevoerd en worden daarom niet geaccepteerd door de doel-e-mailorganisatie.

Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waaraan u e-mail wilt verzenden. Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht. Microsoft-ondersteuning kan mogelijk niet verder helpen.
