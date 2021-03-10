---
title: Gebruikersbeleid/postvakinstellingen herstellen
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693304"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="72c66-102">Gebruikersbeleid/postvakinstellingen herstellen</span><span class="sxs-lookup"><span data-stu-id="72c66-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="72c66-103">De instellingen voor ongewenste e-mail in het postvak zijn van invloed op dit bericht.</span><span class="sxs-lookup"><span data-stu-id="72c66-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="72c66-104">Ga als volgt te werk om de instellingen te controleren:</span><span class="sxs-lookup"><span data-stu-id="72c66-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="72c66-105">Start exchange-beheershell.</span><span class="sxs-lookup"><span data-stu-id="72c66-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="72c66-106">Zie De [Exchange-beheershell openen](https://go.microsoft.com/fwlink/?linkid=2101432)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="72c66-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="72c66-107">Voer deze opdracht uit (met het e-mailadres van de gebruiker):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="72c66-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="72c66-108">Controleer of het e-mailadres van de afzender deel uitmaakt van **TrustedSendersAndDomains** of **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="72c66-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="72c66-109">Als het e-mailadres in een van de lijsten staat, moet u dit mogelijk verwijderen.</span><span class="sxs-lookup"><span data-stu-id="72c66-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="72c66-110">Zie [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="72c66-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
