---
title: Problemen met SMTP-verificatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264367"
---
# <a name="solving-smtp-authentication-issues"></a>Problemen met SMTP-verificatie oplossen

Als u fouten 5.7.57 of 5.7.3 krijgt wanneer u SMTP-e-mail probeert te verzenden en verifiëren met een client of toepassing, zijn er een paar dingen die u moet controleren:

- Geverifieerde SMTP-indiening kan worden uitgeschakeld in uw tenant of in het postvak dat u probeert te gebruiken (controleer beide instellingen). Zie [Verificatie client SMTP-indiening inschakelen of uitschakelen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)voor meer informatie.

- Controleer of [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) zijn ingeschakeld voor uw tenant. als dit is ingeschakeld, mislukt SMTP-verificatie met basisverificatie (ook bekend als legacy, dit gebruikt gebruikersnaam en wachtwoord).
