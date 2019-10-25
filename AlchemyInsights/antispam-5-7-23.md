---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682096"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met de bezorging van e-mail oplossen voor foutcode 5.7.23

Controleer de SPF DNS-record voor uw domein op een openbaar beschikbare SPF of DNS record checker op het web.

Controleer of het uitgaande bericht niet is geïdentificeerd als spam door Office 365 en doorgestuurd via de [groep met hoog risico-levering](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Berichten in de groep met hoog risico levering niet doorgeven SPF controles en daarom niet worden geaccepteerd door de organisatie van de bestemming e-mailadres.

Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u probeert e-mail te verzenden. Noteer de gedetailleerde externe fout die beschikbaar is in het Bounce-bericht.  Ondersteuning voor Office 365 kan mogelijk niet verder helpen.