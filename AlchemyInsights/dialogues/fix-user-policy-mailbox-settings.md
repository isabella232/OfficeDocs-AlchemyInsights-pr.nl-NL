---
title: Gebruikersbeleid/postvakinstellingen herstellen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693304"
---
# <a name="fix-user-policymailbox-settings"></a>Gebruikersbeleid/postvakinstellingen herstellen

De instellingen voor ongewenste e-mail in het postvak zijn van invloed op dit bericht. Ga als volgt te werk om de instellingen te controleren:

1. Start exchange-beheershell. Zie De [Exchange-beheershell openen](https://go.microsoft.com/fwlink/?linkid=2101432)voor meer informatie.
2. Voer deze opdracht uit (met het e-mailadres van de gebruiker):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Controleer of het e-mailadres van de afzender deel uitmaakt van **TrustedSendersAndDomains** of **BlockedSendersAndDomains.** Als het e-mailadres in een van de lijsten staat, moet u dit mogelijk verwijderen. Zie [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)voor meer informatie.
