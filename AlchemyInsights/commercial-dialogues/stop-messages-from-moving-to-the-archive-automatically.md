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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744670"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="ed60e-102">Voorkomen dat berichten automatisch naar het archief worden verplaatst</span><span class="sxs-lookup"><span data-stu-id="ed60e-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="ed60e-103">Als u een bewaarbeleid gebruikt, kunt u de bewaarleeftijd in dat beleid wijzigen om te voorkomen dat berichten automatisch worden gearchiveren.</span><span class="sxs-lookup"><span data-stu-id="ed60e-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="ed60e-104">Hier ziet u hoe dat gaat:</span><span class="sxs-lookup"><span data-stu-id="ed60e-104">Here's how:</span></span>

1. <span data-ttu-id="ed60e-105">Kies in [het Exchange-beheercentrum](https://go.microsoft.com/fwlink/?linkid=2059104) compliancebeheerbewaringslabels.  >  </span><span class="sxs-lookup"><span data-stu-id="ed60e-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="ed60e-106">Zoek de bewaartag Verplaatsen naar archiveren.</span><span class="sxs-lookup"><span data-stu-id="ed60e-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="ed60e-107">Wijzig in de bewaartag de bewaarperiode (archiefperiode) in **Nooit** om te voorkomen dat items automatisch worden gearchiveerd door een bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="ed60e-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="ed60e-108">Hierdoor wordt de archiefinstelling voor alle postvakken gewijzigd, met deze bewaartag die op deze postvakken is toegepast.</span><span class="sxs-lookup"><span data-stu-id="ed60e-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
