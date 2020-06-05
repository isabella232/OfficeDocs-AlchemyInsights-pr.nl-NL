---
title: Problemen met gebeurtenissen oplossen via e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569006"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="fe361-102">Problemen met gebeurtenissen oplossen via e-mail</span><span class="sxs-lookup"><span data-stu-id="fe361-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="fe361-103">Controleer of de functie is ingeschakeld voor het postvak: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="fe361-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="fe361-104">Kijk dan naar de 'Gebeurtenissen uit e-mail' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="fe361-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="fe361-105">Zoek in de logboeken 'Gebeurtenissen uit e-mail' de InternetMessageId die overeenkomt met het item in het postvak.</span><span class="sxs-lookup"><span data-stu-id="fe361-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="fe361-106">De TrustScore bepaalt of het item is toegevoegd of niet.</span><span class="sxs-lookup"><span data-stu-id="fe361-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="fe361-107">Gebeurtenissen worden alleen toegevoegd als de TrustScore = "Vertrouwd" wordt.</span><span class="sxs-lookup"><span data-stu-id="fe361-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="fe361-108">De TrustScore wordt bepaald door de eigenschappen SPF, Dkim of Dmarc, die zich in de berichtkoptekst bevinden.</span><span class="sxs-lookup"><span data-stu-id="fe361-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="fe361-109">Ga als u deze eigenschappen wilt bekijken:</span><span class="sxs-lookup"><span data-stu-id="fe361-109">To view these properties:</span></span>

<span data-ttu-id="fe361-110">**Bureaublad Outlook**</span><span class="sxs-lookup"><span data-stu-id="fe361-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="fe361-111">Het item openen</span><span class="sxs-lookup"><span data-stu-id="fe361-111">Open the item</span></span>
- <span data-ttu-id="fe361-112">Bestands -> Eigenschappen -> internetkoppen</span><span class="sxs-lookup"><span data-stu-id="fe361-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="fe361-113">of</span><span class="sxs-lookup"><span data-stu-id="fe361-113">or</span></span>

<span data-ttu-id="fe361-114">**MFCMapi MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="fe361-114">**MFCMapi**</span></span>

- <span data-ttu-id="fe361-115">Navigeren naar het item in het postvak IN</span><span class="sxs-lookup"><span data-stu-id="fe361-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="fe361-116">Zoek naar PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="fe361-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="fe361-117">Deze eigenschappen worden bepaald en geregistreerd tijdens transport en routing.</span><span class="sxs-lookup"><span data-stu-id="fe361-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="fe361-118">Voor verdere probleemoplossing moet u mogelijk de transportondersteuning opvolgen over de fouten in SPF, DKIM en.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="fe361-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>