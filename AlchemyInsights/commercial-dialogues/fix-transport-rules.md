---
title: Transportregels oplossen
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744844"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="a0de4-102">Transportregels oplossen</span><span class="sxs-lookup"><span data-stu-id="a0de4-102">Fix transport rules</span></span>

<span data-ttu-id="a0de4-103">Dit bericht is beïnvloed door een aangepaste e-mailstroomregel.</span><span class="sxs-lookup"><span data-stu-id="a0de4-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="a0de4-104">Ga als volgt te werk om de exacte regel te bekijken:</span><span class="sxs-lookup"><span data-stu-id="a0de4-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="a0de4-105">Noteer in de resultaten van de inzending onder **Aanvullende informatie** de **GUID** of de **naam van het beleid.**</span><span class="sxs-lookup"><span data-stu-id="a0de4-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="a0de4-106">Start Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="a0de4-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="a0de4-107">Zie De Exchange Management Shell openen voor [meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="a0de4-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="a0de4-108">Voer deze opdracht uit (met de GUID van uw inzending):  **Get-TransportRule -identity "GUID" | fl \* Beschrijving**\*</span><span class="sxs-lookup"><span data-stu-id="a0de4-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="a0de4-109">Bekijk de beschrijving om de geconfigureerde voorwaarden te bekijken die van invloed zijn op het bericht.</span><span class="sxs-lookup"><span data-stu-id="a0de4-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="a0de4-110">Zie [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a0de4-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
