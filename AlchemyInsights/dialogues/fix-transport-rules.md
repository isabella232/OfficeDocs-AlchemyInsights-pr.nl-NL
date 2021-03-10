---
title: Transportregels herstellen
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693295"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="9b084-102">Transportregels herstellen</span><span class="sxs-lookup"><span data-stu-id="9b084-102">Fix transport rules</span></span>

<span data-ttu-id="9b084-103">Dit bericht is beïnvloed door een aangepaste regel voor de e-mailstroom.</span><span class="sxs-lookup"><span data-stu-id="9b084-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="9b084-104">Ga als volgt te werk om de exacte regel te controleren:</span><span class="sxs-lookup"><span data-stu-id="9b084-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="9b084-105">Let in de resultaten van de indiening onder **Aanvullende informatie** op de **GUID** of de **beleidsnaam.**</span><span class="sxs-lookup"><span data-stu-id="9b084-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="9b084-106">Start exchange-beheershell.</span><span class="sxs-lookup"><span data-stu-id="9b084-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="9b084-107">Zie De [Exchange-beheershell openen](https://go.microsoft.com/fwlink/?linkid=2101432)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9b084-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="9b084-108">Voer deze opdracht uit (met de GUID van uw inzending):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="9b084-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="9b084-109">Bekijk de beschrijving om de geconfigureerde voorwaarden te bekijken die van invloed zijn op het bericht.</span><span class="sxs-lookup"><span data-stu-id="9b084-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="9b084-110">Zie [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9b084-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
