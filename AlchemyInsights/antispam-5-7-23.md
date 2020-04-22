---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676492"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met e-mailbezorging oplossen voor foutcode 5.7.23

Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op internet.

Controleer of het uitgaande bericht niet door Microsoft als spam is geïdentificeerd en door de [groep levering met een hoog risico](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)is doorgestuurd. Berichten in de groep Levering met een hoog risico worden niet door de SPF-controles gehaald en worden daarom niet geaccepteerd door de e-mailorganisatie van de bestemming.

Als het probleem blijft bestaan, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u e-mail probeert te verzenden. Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht. Microsoft-ondersteuning kan mogelijk niet verder helpen.
