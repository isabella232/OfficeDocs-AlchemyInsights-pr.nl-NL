---
title: Beleid voor het delen van agenda's
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372994"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Beleidsfout bij het delen van een agenda

1. Doe een van de volgende handelingen, naar gelang van het geval voor uw situatie:
    - Maak verbinding met Exchange Online met Remote PowerShell. Zie [Verbinding maken met Exchange Online met Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)voor meer informatie.
    - Open de Exchange Management Shell op de on-premises server.
2. Bepaal het beleid voor delen dat aan de gebruiker is toegewezen. Voer hiervoor de volgende opdracht uit en noteer het geretourneerde beleid:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Werk het beleid voor delen voor de gebruiker bij. Volg deze stappen om dit te doen:
    - Open het Exchange-beheercentrum.
    - Klik **op Organisatie**en dubbelklik op het beleid dat aan de gebruiker is toegewezen onder Individueel **delen**. Dit is het beleid dat is geretourneerd in stap 2.
    - Selecteer op de pagina Regel delen het niveau voor het delen van agenda's dat u wilt toestaan onder **Opgeven welke informatie u wilt delen**; klik **op Opslaan**.

Voor meer informatie zie: ["Beleid staat niet toe dat machtigingen op dit niveau worden verleend aan een of meer van de ontvanger(s)" fout wanneer de gebruiker probeert om agenda te delen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
