---
title: Instellingen voor gebruikersbeleid/postvak oplossen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744841"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="27c21-102">Instellingen voor gebruikersbeleid/postvak oplossen</span><span class="sxs-lookup"><span data-stu-id="27c21-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="27c21-103">De instellingen voor ongewenste e-mail in het postvak zijn van invloed op dit bericht.</span><span class="sxs-lookup"><span data-stu-id="27c21-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="27c21-104">Ga als volgt te werk om de instellingen te bekijken:</span><span class="sxs-lookup"><span data-stu-id="27c21-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="27c21-105">Start Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="27c21-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="27c21-106">Zie De Exchange Management Shell openen voor [meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="27c21-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="27c21-107">Voer deze opdracht uit (met het e-mailadres van de gebruiker):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="27c21-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="27c21-108">Controleer of het e-mailadres van de afzender deel uitmaakt van **TrustedSendersAndDomains** of **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="27c21-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="27c21-109">Als het e-mailadres in een van de lijsten staat, moet u het mogelijk verwijderen.</span><span class="sxs-lookup"><span data-stu-id="27c21-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="27c21-110">Zie [Set-MailboxJunkEmailConfiguration (Set-MailboxJunkEmailConfiguration) voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="27c21-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
