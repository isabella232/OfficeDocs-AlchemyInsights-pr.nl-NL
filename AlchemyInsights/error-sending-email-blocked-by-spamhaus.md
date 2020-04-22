---
title: Fout verzenden e-mail geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714253"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="4dd2c-102">Fout verzenden e-mail: Clienthost geblokkeerd met Spamhaus</span><span class="sxs-lookup"><span data-stu-id="4dd2c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="4dd2c-103">Het IP-adres dat het bericht heeft verzonden, staat op een bloklijst die eigendom is van [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="4dd2c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="4dd2c-104">Redenen om geblokkeerd te worden door Spamhaus zijn gecompromitteerde accounts, gecompromitteerde machines die een openbaar IP-adres delen en internetserviceprovider (ISP)-beleid.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="4dd2c-105">Mogelijke oplossingen zijn:</span><span class="sxs-lookup"><span data-stu-id="4dd2c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="4dd2c-106">Voor geblokkeerde binnenkomende berichten waarin u de brone-mailserver beheert, moet u de oorzaak bepalen en het blok verwijderen van de Spamhaus-website.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="4dd2c-107">Voor geblokkeerde binnenkomende berichten waarbij het ip-adres van de bron van iemand anders is, moet de adreseigenaar het blok verwijderen van de Spamhaus-website.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="4dd2c-108">Als het IP-adres op de Beleidsbloklijst (PBL) staat, kan de eigenaar een ander statisch IP-adres toewijzen of het adres van het PBL verwijderen.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="4dd2c-109">Voor geblokkeerde uitgaande berichten uit uw domein die zijn verbonden met Microsoft, u deze fout ontvangen als de berichten worden doorgestuurd via een service van derden.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="4dd2c-110">U een WHOIS-opzoektool gebruiken om de eigenaar van het geblokkeerde IP-adres te vinden.</span><span class="sxs-lookup"><span data-stu-id="4dd2c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
