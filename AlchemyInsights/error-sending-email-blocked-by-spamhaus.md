---
title: Fout bij het verzenden van e-mailadres is geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527127"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="e6300-102">Fout bij het verzenden van e-mail: Client host is geblokkeerd met behulp van Spamhaus</span><span class="sxs-lookup"><span data-stu-id="e6300-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="e6300-103">Het IP-adres voor het bericht is op een lijst met geblokkeerde websites die eigendom zijn van [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="e6300-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="e6300-104">Redenen voor zijn geblokkeerd in de Spamhaus zijn gekraakte accounts, machines, delen van een openbaar IP-adres en een Internet Service Provider (ISP) beleid in gevaar gebracht.</span><span class="sxs-lookup"><span data-stu-id="e6300-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="e6300-105">Mogelijke oplossingen zijn:</span><span class="sxs-lookup"><span data-stu-id="e6300-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="e6300-106">Voor binnenkomende berichten geblokkeerd voor Office 365, waar u de bron-e-mailserver beheren, moet u de oorzaak en het blok verwijderen vanaf de website van Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="e6300-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="e6300-107">Voor binnenkomende berichten geblokkeerd met Office 365 waar het bron-IP-adres van iemand anders, moet de eigenaar van het adres het blok verwijderen vanaf de website van Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="e6300-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="e6300-108">Als het IP-adres op het beleid blokkeren lijst (PBL), kan de eigenaar een andere statische IP-adres toewijzen of verwijderen van het adres van de PBL.</span><span class="sxs-lookup"><span data-stu-id="e6300-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="e6300-109">Voor uitgaande berichten uit uw domein van Office 365 geblokkeerd, kunt u deze fout optreden als de berichten worden gerouteerd via een 3e partij.</span><span class="sxs-lookup"><span data-stu-id="e6300-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="e6300-110">Een WHOIS lookup tool kunt u de eigenaar van de geblokkeerde IP-adres vinden.</span><span class="sxs-lookup"><span data-stu-id="e6300-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
