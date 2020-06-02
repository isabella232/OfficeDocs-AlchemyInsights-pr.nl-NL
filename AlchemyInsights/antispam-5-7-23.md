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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506438"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met e-mailbezorging oplossen voor foutcode 5.7.23

Controleer de DNS-record SPF voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op het web.

Controleer of het uitgaande bericht niet door Microsoft als spam is geïdentificeerd en door de [pool met levering met een hoog risico is](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)doorgestuurd. Berichten in de pool met levering met een hoog risico worden niet doorgegeven aan SPF-controles en worden daarom niet geaccepteerd door de e-mailorganisatie voor bestemmingen.

Als het probleem blijft bestaan, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u e-mail probeert te verzenden. Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht. Microsoft-ondersteuning kan mogelijk niet verder helpen.
