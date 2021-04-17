---
title: Problemen met gebeurtenissen vanuit e-mail oplossen
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834834"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="6cb70-102">Problemen met gebeurtenissen vanuit e-mail oplossen</span><span class="sxs-lookup"><span data-stu-id="6cb70-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="6cb70-103">Controleer of de functie is ingeschakeld voor het postvak: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="6cb70-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="6cb70-104">Bekijk vervolgens de logboeken 'Gebeurtenissen uit e-mail' **Export-MailboxDiagnosticLogs<mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="6cb70-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="6cb70-105">Zoek in de logboeken 'Gebeurtenissen uit e-mail' de InternetMessageId die overeenkomt met het item in het postvak.</span><span class="sxs-lookup"><span data-stu-id="6cb70-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="6cb70-106">De TrustScore bepaalt of het item wordt toegevoegd of niet.</span><span class="sxs-lookup"><span data-stu-id="6cb70-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="6cb70-107">Gebeurtenissen worden alleen toegevoegd als de TrustScore = 'Trusted'.</span><span class="sxs-lookup"><span data-stu-id="6cb70-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="6cb70-108">De TrustScore wordt bepaald door de SPF-, Dkim- of Dmarc-eigenschappen, die in de berichtkop staan.</span><span class="sxs-lookup"><span data-stu-id="6cb70-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="6cb70-109">Om deze eigenschappen te bekijken:</span><span class="sxs-lookup"><span data-stu-id="6cb70-109">To view these properties:</span></span>

<span data-ttu-id="6cb70-110">**Bureaubladversie van Outlook**</span><span class="sxs-lookup"><span data-stu-id="6cb70-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="6cb70-111">Het item openen</span><span class="sxs-lookup"><span data-stu-id="6cb70-111">Open the item</span></span>
- <span data-ttu-id="6cb70-112">Bestand -> Eigenschappen -> Internetkoppen</span><span class="sxs-lookup"><span data-stu-id="6cb70-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="6cb70-113">of</span><span class="sxs-lookup"><span data-stu-id="6cb70-113">or</span></span>

<span data-ttu-id="6cb70-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="6cb70-114">**MFCMapi**</span></span>

- <span data-ttu-id="6cb70-115">Naar het item in het Postvak IN gaan</span><span class="sxs-lookup"><span data-stu-id="6cb70-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="6cb70-116">Zoek naar PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="6cb70-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="6cb70-117">Deze eigenschappen worden bepaald en vastgelegd tijdens transport en routering.</span><span class="sxs-lookup"><span data-stu-id="6cb70-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="6cb70-118">Voor verdere probleemoplossing moet u mogelijk contact opnemen met Transport Support over de fouten in SPF, DKIM en/of DMARC.</span><span class="sxs-lookup"><span data-stu-id="6cb70-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>