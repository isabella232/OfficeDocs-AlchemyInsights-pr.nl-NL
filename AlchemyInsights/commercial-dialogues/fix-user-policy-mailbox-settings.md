---
title: Instellingen voor gebruikersbeleid/postvak oplossen
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744841"
---
# <a name="fix-user-policymailbox-settings"></a>Instellingen voor gebruikersbeleid/postvak oplossen

De instellingen voor ongewenste e-mail in het postvak zijn van invloed op dit bericht. Ga als volgt te werk om de instellingen te bekijken:

1. Start Exchange Management Shell. Zie De Exchange Management Shell openen voor [meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Voer deze opdracht uit (met het e-mailadres van de gebruiker):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Controleer of het e-mailadres van de afzender deel uitmaakt van **TrustedSendersAndDomains** of **BlockedSendersAndDomains.** Als het e-mailadres in een van de lijsten staat, moet u het mogelijk verwijderen. Zie [Set-MailboxJunkEmailConfiguration (Set-MailboxJunkEmailConfiguration) voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101047)
