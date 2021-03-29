---
title: Controleren op doorsturen van adressen in postvakken
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403306"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c5978-102">Controleren op doorsturen van adressen in postvakken</span><span class="sxs-lookup"><span data-stu-id="c5978-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c5978-103">Soms sturen hackers e-mailberichten van gebruikers door naar zichzelf, dus eerst controleren we of we adressen en regels in het postvak doorsturen.</span><span class="sxs-lookup"><span data-stu-id="c5978-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c5978-104">Vervolgens controleren we de auditlogboeken.</span><span class="sxs-lookup"><span data-stu-id="c5978-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c5978-105">U kunt als volgende controleren op doorsturen van adressen:</span><span class="sxs-lookup"><span data-stu-id="c5978-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c5978-106">Selecteer **Gebruikers**  >  **Actieve gebruikers**.</span><span class="sxs-lookup"><span data-stu-id="c5978-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c5978-107">Selecteer de gebruiker van wie het account is gehackt.</span><span class="sxs-lookup"><span data-stu-id="c5978-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c5978-108">Vouw in het flyout dat wordt weergegeven **E-mailinstellingen** uit en klik vervolgens **op Bewerken** voor **e-mail doorsturen.**</span><span class="sxs-lookup"><span data-stu-id="c5978-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c5978-109">Verwijder doorsturende adressen die u niet herkent.</span><span class="sxs-lookup"><span data-stu-id="c5978-109">Remove any forwarding addresses you don't recognize.</span></span>