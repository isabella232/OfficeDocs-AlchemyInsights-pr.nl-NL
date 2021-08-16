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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034749"
---
# <a name="fix-transport-rules"></a>Transportregels oplossen

Dit bericht is beïnvloed door een aangepaste e-mailstroomregel. Ga als volgt te werk om de exacte regel te bekijken:

1. Noteer in de resultaten van de inzending onder **Aanvullende informatie** de **GUID** of de **naam van het beleid.**
2. Start Exchange Management Shell. Zie De Exchange [Management Shell openen voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Voer deze opdracht uit (met de GUID van uw inzending):  **Get-TransportRule -identity "GUID" | fl * Beschrijving***
4. Bekijk de beschrijving om de geconfigureerde voorwaarden te bekijken die van invloed zijn op het bericht.

Zie [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)voor meer informatie.
