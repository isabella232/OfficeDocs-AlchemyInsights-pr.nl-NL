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
# <a name="fix-transport-rules"></a>Transportregels herstellen

Dit bericht is beïnvloed door een aangepaste regel voor de e-mailstroom. Ga als volgt te werk om de exacte regel te controleren:

1. Let in de resultaten van de indiening onder **Aanvullende informatie** op de **GUID** of de **beleidsnaam.**
2. Start exchange-beheershell. Zie De [Exchange-beheershell openen](https://go.microsoft.com/fwlink/?linkid=2101432)voor meer informatie.
3. Voer deze opdracht uit (met de GUID van uw inzending):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Bekijk de beschrijving om de geconfigureerde voorwaarden te bekijken die van invloed zijn op het bericht.

Zie [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)voor meer informatie.
