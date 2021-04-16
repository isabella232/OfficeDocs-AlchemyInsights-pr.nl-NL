---
title: Fout bij het verzenden van e-mail die is geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813719"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3538f-102">Fout bij het verzenden van e-mail: Clienthost geblokkeerd met Spamhaus</span><span class="sxs-lookup"><span data-stu-id="3538f-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3538f-103">Het IP-adres dat het bericht heeft verzonden, staat in een bloklijst die eigendom is van [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="3538f-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3538f-104">Redenen voor het blokkeren door Spamhaus zijn gecompromitteerde accounts, gecompromitteerde computers die een openbaar IP-adres delen en internetproviderbeleid.</span><span class="sxs-lookup"><span data-stu-id="3538f-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3538f-105">Mogelijke oplossingen zijn:</span><span class="sxs-lookup"><span data-stu-id="3538f-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3538f-106">Voor geblokkeerde binnenkomende berichten waarin u de bron-e-mailserver controleert, moet u de oorzaak bepalen en het blok verwijderen van de spamhaus-website.</span><span class="sxs-lookup"><span data-stu-id="3538f-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3538f-107">Voor geblokkeerde binnenkomende berichten waarbij het bron-IP-adres van iemand anders is, moet de eigenaar van het adres het blok van de spamhaus-website verwijderen.</span><span class="sxs-lookup"><span data-stu-id="3538f-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3538f-108">Als het IP-adres zich in de lijst met beleidsblokkeringen (PBL) vindt, kan de eigenaar een ander statisch IP-adres toewijzen of het adres uit het PBL verwijderen.</span><span class="sxs-lookup"><span data-stu-id="3538f-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3538f-109">Voor geblokkeerde uitgaande berichten van uw domein die zijn verbonden met Microsoft, kunt u deze fout ontvangen als de berichten worden gerouteerd via een service van derden.</span><span class="sxs-lookup"><span data-stu-id="3538f-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3538f-110">U kunt een WHOIS-zoekprogramma gebruiken om de geblokkeerde eigenaar van het IP-adres te zoeken.</span><span class="sxs-lookup"><span data-stu-id="3538f-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
