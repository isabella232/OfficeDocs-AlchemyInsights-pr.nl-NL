---
title: Problemen met SMTP-verificatie oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826410"
---
# <a name="solving-smtp-authentication-issues"></a>Problemen met SMTP-verificatie oplossen

Als u fouten 5.7.57 of 5.7.3 krijgt bij het verzenden van SMTP-e-mail en zich wilt verifiëren met een client of toepassing, zijn er een paar dingen die u moet controleren:

- Geverifieerde SMTP-inzending kan worden uitgeschakeld in uw tenant of in het postvak dat u wilt gebruiken (controleer beide instellingen). Zie Geverifieerde [SMTP-inzending voor client](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)in- of uitschakelen voor meer informatie.

- Controleer of [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) zijn ingeschakeld voor uw tenant. Als dit is ingeschakeld, mislukt SMTP-verificatie met basisverificatie (ook wel bekend als oudere verificatie; hiervoor wordt gebruikersnaam en wachtwoord gebruikt) mislukt.
