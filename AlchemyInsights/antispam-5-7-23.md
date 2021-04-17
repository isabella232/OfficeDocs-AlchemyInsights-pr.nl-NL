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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821406"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met e-mailbezorging oplossen voor foutcode 5.7.23

Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op het web.

Controleer of het uitgaande bericht niet is geïdentificeerd als spam door Microsoft en door de groep met hoge [risicobezorging is gerouteerd.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Berichten in de groep Bezorging met hoog risico worden niet door SPF-controles uitgevoerd en worden daarom niet geaccepteerd door de doel-e-mailorganisatie.

Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waaraan u e-mail wilt verzenden. Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht. Microsoft-ondersteuning kan mogelijk niet verder helpen.
