---
title: Controleren op doorsturen van adressen in postvakken
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481803"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="03098-102">Controleren op doorsturen van adressen in postvakken</span><span class="sxs-lookup"><span data-stu-id="03098-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="03098-103">Soms sturen hackers e-mailberichten van gebruikers door naar zichzelf, dus eerst wordt er gekeken of er e-mailadressen en regels voor het postvak worden doorgestuurd.</span><span class="sxs-lookup"><span data-stu-id="03098-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="03098-104">Vervolgens controleren we de auditlogboeken.</span><span class="sxs-lookup"><span data-stu-id="03098-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="03098-105">U kunt als volgende controleren of er doorgestuurde adressen zijn:</span><span class="sxs-lookup"><span data-stu-id="03098-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="03098-106">Gebruikers **selecteren**  >  **die actief zijn.**</span><span class="sxs-lookup"><span data-stu-id="03098-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="03098-107">Selecteer de gebruiker van wie het account is gehackt.</span><span class="sxs-lookup"><span data-stu-id="03098-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="03098-108">Vouw in de flyout die wordt weergegeven **e-mailinstellingen** uit en klik op **Bewerken** voor e-mail **doorsturen.**</span><span class="sxs-lookup"><span data-stu-id="03098-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="03098-109">Verwijder alle doorgestuurde adressen die u niet herkent.</span><span class="sxs-lookup"><span data-stu-id="03098-109">Remove any forwarding addresses you don't recognize.</span></span>