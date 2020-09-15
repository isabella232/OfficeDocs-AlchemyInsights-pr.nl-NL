---
title: Beleid voor het delen van een 618-agenda
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684225"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Beleidsfout bij het delen van een agenda

1. Voer een van de volgende handelingen uit, afhankelijk van uw situatie:
    - Maak verbinding met Exchange Online via externe PowerShell. Zie [verbinding maken met Exchange Online via externe PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)voor meer informatie.
    - Open de Exchange-beheer shell op de lokale server.
2. Bepaal het beleid voordelen dat is toegewezen aan de gebruiker. Als u dit wilt doen, voert u de volgende opdracht uit en noteert u het geretourneerde beleid:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Het beleid voor het delen van de gebruiker bijwerken. Ga hiervoor als volgt te werk:
    - Open het Exchange-beheercentrum.
    - Klik op **organisatie**en dubbelklik vervolgens op het beleid dat is toegewezen aan de gebruiker onder **afzonderlijk delen**. Dit is het beleid dat u in stap 2 hebt geretourneerd.
    - Selecteer op de pagina regel voordelen het niveau voor het delen van de agenda dat u wilt toestaan onder **opgeven welke gegevens u wilt delen**. Selecteer **Opslaan**.

Zie voor meer informatie: [' beleid staat het toekennen van machtigingen op dit niveau toe aan een of meer van de geadresseerde (n) wanneer de gebruiker probeert de agenda te delen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
