---
title: Hulp nodig bij het verzenden van e-maillimieten?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836274"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="7cd44-102">Hulp nodig bij het verzenden van e-maillimieten?</span><span class="sxs-lookup"><span data-stu-id="7cd44-102">Need help with email sending limits?</span></span>

<span data-ttu-id="7cd44-103">Hieronder vindt u de **standaard verzendlimieten** die in de service worden opgelegd.</span><span class="sxs-lookup"><span data-stu-id="7cd44-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="7cd44-104">Meer informatie over deze limieten vindt u [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="7cd44-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="7cd44-105">Om de bezorging van ongevraagde bulkberichten te ontmoedigen, passen we limieten per gebruiker **van geadresseerden toe op alle uitgaande en interne berichten**.</span><span class="sxs-lookup"><span data-stu-id="7cd44-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="7cd44-106">Voor alle SKU's is deze limiet **10.000 ontvangers per dag**.</span><span class="sxs-lookup"><span data-stu-id="7cd44-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="7cd44-107">Klanten die legitieme bulk commerciële e-mail moeten verzenden (bijvoorbeeld nieuwsbrieven), moeten gebruikmaken van externe providers die gespecialiseerd zijn in deze services.</span><span class="sxs-lookup"><span data-stu-id="7cd44-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="7cd44-108">**Opmerking**: zodra de limiet is bereikt, kunnen geen berichten meer vanuit het postvak worden verzonden, tot het aantal geadresseerden aan wie de afgelopen 24 uur berichten zijn verzonden, onder deze limiet is gezakt.</span><span class="sxs-lookup"><span data-stu-id="7cd44-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="7cd44-109">De gebruiker kan tot dat moment geen berichten verzenden.</span><span class="sxs-lookup"><span data-stu-id="7cd44-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="7cd44-110">De berichtsnelheidslimiet van **30 berichten per minuut** wordt toegepast op alle SKU's.</span><span class="sxs-lookup"><span data-stu-id="7cd44-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="7cd44-111">Hiermee wordt bepaald hoeveel berichten een gebruiker binnen een bepaalde periode kan verzenden vanaf zijn of haar Exchange Online-account.</span><span class="sxs-lookup"><span data-stu-id="7cd44-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="7cd44-112">Het **maximum aantal geadresseerden dat is toegestaan in de velden Aan, CC en BCC** voor één e-mailbericht, voor alle SKU's, is **1000 geadresseerden**.</span><span class="sxs-lookup"><span data-stu-id="7cd44-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="7cd44-113">Ga [hierheen](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228) om deze limiet aan te passen.</span><span class="sxs-lookup"><span data-stu-id="7cd44-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
