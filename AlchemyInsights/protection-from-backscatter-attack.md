---
title: Beveiliging tegen backscatter-aanval
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035410"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="751dc-102">Beveiliging tegen backscatter-aanval</span><span class="sxs-lookup"><span data-stu-id="751dc-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="751dc-103">Backscatter is niet-bezorgingsrapporten (ook wel NDR's of niet-bezorgde berichten genoemd) die u ontvangt voor berichten die u niet hebt verzonden.</span><span class="sxs-lookup"><span data-stu-id="751dc-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="751dc-104">Spammers vervalsen (spoof) het **Van:-adres** van hun berichten en ze gebruiken vaak echte e-mailadressen om hun berichten geloofwaardig te maken.</span><span class="sxs-lookup"><span data-stu-id="751dc-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="751dc-105">Dus wanneer spammers onvermijdelijk berichten verzenden naar niet-bestaande geadresseerden, wordt de doel-e-mailserver in feite misleid om het niet-verkeerbare bericht in een NDR terug te sturen naar de vervalste afzender in het **Adres van:** van.</span><span class="sxs-lookup"><span data-stu-id="751dc-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="751dc-106">Aanvullende informatie vindt u in [Backscatter in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="751dc-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="751dc-107">**Backscatterbeveiliging inschakelen**</span><span class="sxs-lookup"><span data-stu-id="751dc-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="751dc-108">Als u backscatterbeveiliging wilt inschakelen, volgt u het onderstaande pad.</span><span class="sxs-lookup"><span data-stu-id="751dc-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="751dc-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to "On"**</span><span class="sxs-lookup"><span data-stu-id="751dc-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="751dc-110">Als u denkt dat een account is gehackt, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="751dc-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="751dc-111">Reageren op een gehackt e-mailaccount</span><span class="sxs-lookup"><span data-stu-id="751dc-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="751dc-112">Geblokkeerde gebruikers verwijderen uit de portal Beperkte gebruikers in Office 365</span><span class="sxs-lookup"><span data-stu-id="751dc-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



