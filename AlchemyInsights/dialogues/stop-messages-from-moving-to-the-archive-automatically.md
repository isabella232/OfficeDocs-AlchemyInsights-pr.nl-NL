---
title: Voorkomen dat berichten automatisch naar het archief worden verplaatst
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525105"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="62263-102">Voorkomen dat berichten automatisch naar het archief worden verplaatst</span><span class="sxs-lookup"><span data-stu-id="62263-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="62263-103">Als u een bewaarbeleid gebruikt, kunt u de bewaartermijn in dat beleid wijzigen om te voorkomen dat berichten automatisch worden gearchiveren.</span><span class="sxs-lookup"><span data-stu-id="62263-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="62263-104">Hier ziet u hoe dat gaat:</span><span class="sxs-lookup"><span data-stu-id="62263-104">Here's how:</span></span>

1. <span data-ttu-id="62263-105">Kies in [het Exchange-beheercentrum](https://go.microsoft.com/fwlink/?linkid=2059104)labels **voor bewaarbeleid** voor  >  **nalevingsbeheer.**</span><span class="sxs-lookup"><span data-stu-id="62263-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="62263-106">Zoek de tag Verplaatsen naar archiefbewaring.</span><span class="sxs-lookup"><span data-stu-id="62263-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="62263-107">Wijzig in de bewaartag de bewaarperiode (archiefperiode) in **Nooit** te stoppen dat items automatisch worden gearchiveerd door een bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="62263-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="62263-108">Hiermee verandert u de archiefinstelling voor alle postvakken waar deze bewaartag op is toegepast.</span><span class="sxs-lookup"><span data-stu-id="62263-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
