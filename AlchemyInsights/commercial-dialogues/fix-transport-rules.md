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
# <a name="fix-transport-rules"></a>Transportregels oplossen

Dit bericht is beïnvloed door een aangepaste e-mailstroomregel. Ga als volgt te werk om de exacte regel te bekijken:

1. Noteer in de resultaten van de inzending onder **Aanvullende informatie** de **GUID** of de **naam van het beleid.**
2. Start Exchange Management Shell. Zie De Exchange Management Shell openen voor [meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Voer deze opdracht uit (met de GUID van uw inzending):  **Get-TransportRule -identity "GUID" | fl * Beschrijving***
4. Bekijk de beschrijving om de geconfigureerde voorwaarden te bekijken die van invloed zijn op het bericht.

Zie [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)voor meer informatie.
