---
title: Hulp nodig bij het verzenden van e-maillimieten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357546"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="70707-102">Hulp nodig bij het verzenden van e-maillimieten?</span><span class="sxs-lookup"><span data-stu-id="70707-102">Need help with email sending limits?</span></span>

<span data-ttu-id="70707-103">Hieronder vindt u de **ontwerp-verzendlimieten** die in de service worden afgedwongen.</span><span class="sxs-lookup"><span data-stu-id="70707-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="70707-104">Meer informatie over deze limieten is [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)gedocumenteerd.</span><span class="sxs-lookup"><span data-stu-id="70707-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="70707-105">Om de levering van ongevraagde bulkberichten te ontmoedigen, passen we tarieflimieten per gebruiker toe **op alle uitgaande en interne berichten.**</span><span class="sxs-lookup"><span data-stu-id="70707-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="70707-106">Voor alle SKU's is deze limiet **10.000 ontvangers per dag.**</span><span class="sxs-lookup"><span data-stu-id="70707-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="70707-107">Klanten die legitieme bulkcommerciële e-mail moeten verzenden (bijvoorbeeld nieuwsbrieven van klanten) moeten gebruik maken van externe providers die gespecialiseerd zijn in deze services.</span><span class="sxs-lookup"><span data-stu-id="70707-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="70707-108">**Opmerking:** Zodra de limiet voor het aantal geadresseerden is bereikt, kunnen berichten niet meer vanuit het postvak worden verzonden totdat het aantal ontvangers dat in de afgelopen 24 uur berichten heeft ontvangen, onder de limiet zakt.</span><span class="sxs-lookup"><span data-stu-id="70707-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="70707-109">De gebruiker kan tot dat moment geen berichten verzenden.</span><span class="sxs-lookup"><span data-stu-id="70707-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="70707-110">De limiet van de berichtsnelheid van **30 berichten per minuut** wordt toegepast op alle SKU's.</span><span class="sxs-lookup"><span data-stu-id="70707-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="70707-111">Dit bepaalt hoeveel berichten een gebruiker binnen een bepaalde periode kan verzenden vanuit zijn Exchange Online-account.</span><span class="sxs-lookup"><span data-stu-id="70707-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="70707-112">Het **maximum aantal geadresseerden dat is toegestaan in de** velden Aan, Cc en BCC voor één e-mailbericht voor alle SKU's, is **1000 ontvangers.**</span><span class="sxs-lookup"><span data-stu-id="70707-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="70707-113">Als u deze limiet wilt aanpassen, gaat u [hier](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)verder .</span><span class="sxs-lookup"><span data-stu-id="70707-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
