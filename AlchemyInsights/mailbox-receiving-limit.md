---
title: Postvak met beperkingsbeperking
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315833"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Postvak met beperkingsbeperking

Microsoft is onlangs begonnen met het afdwingen van de drempel per postvak van 3600 berichten per uur. Zie voor meer informatie [Exchange Online limieten.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 postvakken die binnen een uur meer dan 3600 berichten ontvangen, worden de komende 60 minuten beperkt. 

Daarnaast wordt de limiet voor het aantal paren van afzenders (SRP) toegepast dat berichten blokkeert die door een Microsoft 365 van een specifieke afzender worden ontvangen. Als één afzender meer dan 33% van de totale drempel of 1200 berichten per rollend uur naar een specifieke geadresseerde verzendt, wordt de SRP-limiet in gang gezet en worden berichten van die afzender niet meer geaccepteerd in het postvak. Houd er rekening mee dat:

- Deze limiet is van toepassing op e-mailberichten die zijn ontvangen van andere tenants, on-premises of internet afzenders.
- De bezorging van e-mail aan het postvak wordt de komende 60 minuten geblokkeerd. 
- Afzenders van deze postvakken ontvangen een rapport over niet-bezorging (5.2.121 of 5.2.122) waarin wordt aangegeven dat het postvak de maximumbezorgingsdrempel heeft overschreden. Intra-tenant (e-mail binnen dezelfde tenant) blijft bezorgd.
- Wanneer de SRP-limiet wordt toegepast, blijft het ontvangende postvak berichten van andere afzenders accepteren.

Beheerders kunnen de huidige postvakactiviteit controleren door toegang te krijgen tot een nieuw rapport en inzicht in het Exchange-beheercentrum met de naam 'Postvakken overschrijden ontvangende limieten'. Het inzicht wordt alleen weergegeven als een tenant beledigende postvakken heeft, terwijl het rapport altijd wordt weergegeven in het dashboard, maar leeg is, tenzij een tenant postvakken heeft gewraakt.

Zie Postvakken die het ontvangen van limieten overschrijden inzicht in de nieuwe EAC voor meer informatie over het ontvangen van [inzichten.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Zie Postvakken die het rapport ontvangende limieten overschrijden in het nieuwe EAC voor meer informatie over het overschrijden van de [ontvangstlimieten.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)