---
title: Fout bij verzenden e-mail geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783798"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="8105c-102">Fout bij verzenden e-mail: client host geblokkeerd met behulp van Spamhaus</span><span class="sxs-lookup"><span data-stu-id="8105c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="8105c-103">Het IP-adres dat het bericht heeft verstuurd bevindt zich op een bloklijst met de eigenaar van [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="8105c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="8105c-104">Redenen om te worden geblokkeerd door Spamhaus zijn in gebruik zijnde accounts, het delen van een openbaar IP-adres en een beleidsregels voor internetproviders.</span><span class="sxs-lookup"><span data-stu-id="8105c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="8105c-105">Mogelijke oplossingen zijn:</span><span class="sxs-lookup"><span data-stu-id="8105c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="8105c-106">Voor geblokkeerde inkomende berichten waarop u de bron-e-mailserver beheert, dient u de oorzaak vast te stellen en de blokkering van de Spamhaus-website te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8105c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="8105c-107">Voor geblokkeerde inkomende berichten waarvan het bron-IP-adres lid is van iemand anders, moet de adres eigenaar de blokkering van de Spamhaus-website verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8105c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="8105c-108">Als het IP-adres zich in de lijst met beleids blokkering (PBL) bevindt, kan de eigenaar een ander statisch IP-adres toewijzen of het adres verwijderen uit de PBL.</span><span class="sxs-lookup"><span data-stu-id="8105c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="8105c-109">Voor geblokkeerde uitgaande berichten van uw domein verbonden met Microsoft, kunt u deze fout weergegeven als de berichten worden gerouteerd via een service van een andere leverancier.</span><span class="sxs-lookup"><span data-stu-id="8105c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="8105c-110">U kunt een WHOIS-zoekprogramma gebruiken om de geblokkeerde IP-adres eigenaar te vinden.</span><span class="sxs-lookup"><span data-stu-id="8105c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
