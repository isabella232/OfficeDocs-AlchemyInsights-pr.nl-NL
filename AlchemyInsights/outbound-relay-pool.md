---
title: Uitgaande relaygroep
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381632"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="3151b-102">Uitgaande relaygroep</span><span class="sxs-lookup"><span data-stu-id="3151b-102">Outbound relay pool</span></span>

<span data-ttu-id="3151b-103">Microsoft wijzigt de configuratie voor het doorsturen of doorsturen van e-mail via Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3151b-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="3151b-104">Berichten in bepaalde scenario's worden doorgestuurd of doorgestuurd via Microsoft 365 met een speciale relaygroep.</span><span class="sxs-lookup"><span data-stu-id="3151b-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="3151b-105">Berichten die worden verzonden met behulp van de relaisgroep, kunnen in de map ongewenste e-mail van de geadresseerde komen te staan.</span><span class="sxs-lookup"><span data-stu-id="3151b-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="3151b-106">Zie Uitgaande [bezorgingsgroepen voor meer informatie.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="3151b-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="3151b-107">Als u een scenario wilt vermijden met de relaygroep, moet u ervoor zorgen dat doorgestuurde/doorgestuurde berichten voldoen aan een van de volgende criteria:</span><span class="sxs-lookup"><span data-stu-id="3151b-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="3151b-108">De uitgaande afzender is een geaccepteerd domein van de tenant.</span><span class="sxs-lookup"><span data-stu-id="3151b-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="3151b-109">Sender Policy Framework (SPF) wordt pas weergegeven wanneer het bericht wordt Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3151b-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="3151b-110">DomainKeys Identified Mail (DKIM) op het domein van de P2-afzender wordt weergegeven wanneer het bericht wordt Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3151b-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="3151b-111">Berichten die voldoen aan de bovenstaande criteria, worden niet door de relaygroep verzonden.</span><span class="sxs-lookup"><span data-stu-id="3151b-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="3151b-112">Als de MX-record voor uw domein is gericht op een externe of on-premises server, gebruikt u verbeterde filtering om ervoor te zorgen dat de SPF-validatie juist is voor binnenkomende e-mail en om te voorkomen dat e-mail wordt verzonden via de relaygroep.</span><span class="sxs-lookup"><span data-stu-id="3151b-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="3151b-113">**Hoe kunnen we zien of we worden beïnvloed door de relaisgroep?**</span><span class="sxs-lookup"><span data-stu-id="3151b-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="3151b-114">Als voor uw doorgestuurde of doorgestuurde e-mailberichten een van de bovenstaande criteria wordt gebruikt, worden berichten niet doorgestuurd via de doorgestuurde groep.</span><span class="sxs-lookup"><span data-stu-id="3151b-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="3151b-115">Als een bericht echter via een relaygroep wordt verzonden, is het IP van de uitgaande server in het bereik 40.95.0.0/16 en bevat de naam van de uitgaande server **rly** in de naam.</span><span class="sxs-lookup"><span data-stu-id="3151b-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

