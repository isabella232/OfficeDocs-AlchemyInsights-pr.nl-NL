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
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="1fa89-102">Problemen met SMTP-verificatie oplossen</span><span class="sxs-lookup"><span data-stu-id="1fa89-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="1fa89-103">Als u fouten 5.7.57 of 5.7.3 krijgt bij het verzenden van SMTP-e-mail en zich wilt verifiëren met een client of toepassing, zijn er een paar dingen die u moet controleren:</span><span class="sxs-lookup"><span data-stu-id="1fa89-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="1fa89-104">Geverifieerde SMTP-inzending kan worden uitgeschakeld in uw tenant of in het postvak dat u wilt gebruiken (controleer beide instellingen).</span><span class="sxs-lookup"><span data-stu-id="1fa89-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="1fa89-105">Zie Geverifieerde [SMTP-inzending voor client](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)in- of uitschakelen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1fa89-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="1fa89-106">Controleer of [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) zijn ingeschakeld voor uw tenant. Als dit is ingeschakeld, mislukt SMTP-verificatie met basisverificatie (ook wel bekend als oudere verificatie; hiervoor wordt gebruikersnaam en wachtwoord gebruikt) mislukt.</span><span class="sxs-lookup"><span data-stu-id="1fa89-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
