---
title: DLP-licentiefout voor eindpunt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564481"
---
# <a name="endpoint-dlp-licensing-error"></a>DLP-licentiefout voor eindpunt

Wanneer u de DLP-eindpunten probeert in te stellen, wordt het volgende foutbericht weergegeven:

`Your organization is missing the licenses required to manage these devices`.

Zorg ervoor dat u een van de volgende abonnementen of invoegtoepassingen hebt:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Naleving van Microsoft 365 E5
- Compliance Microsoft 365 A5
- Microsoft 365 E5 Information Protection en governance
- Microsoft 365 A5 Information Protection en governance

> [!NOTE]
> Dit werkt niet voor combinaties van licenties, zoals: Win E5 + O365 E5 + EMS E5. Deze functie kan alleen worden ingesteld door een pure M365 E5-licentie.

Zie [DLP-licentie voor DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) -licentie voor meer informatie over DLP-licenties voor het eindpunt.
