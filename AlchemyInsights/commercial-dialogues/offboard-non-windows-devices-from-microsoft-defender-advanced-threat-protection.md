---
title: Niet-offboard-apparaten Windows Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967796"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Niet-offboard-apparaten Windows Microsoft Defender Advanced Threat Protection (ATP)

Hier ziet u hoe dat gaat:

1. Volg de documentatie van derden voor het loskoppelen van de externe oplossing van Microsoft Defender ATP.
2. Verwijder uit Azure Active Directory tenant machtigingen voor de oplossing van derden:

    1. Meld u aan bij [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Selecteer **Alle services**  >  **Azure Active Directory**  >  **Enterprise Applications**.
    1. Selecteer de toepassing die u wilt offboarden.
    1. Selecteer **Verwijderen**.

Zie [Offboard non-Windows devices voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2143630)
