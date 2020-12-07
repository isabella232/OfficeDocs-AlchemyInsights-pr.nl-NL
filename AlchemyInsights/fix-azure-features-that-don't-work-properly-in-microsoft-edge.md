---
title: Wat u moet doen als Azure-functies niet goed werken in Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583307"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Wat u moet doen als Azure-functies niet goed werken in Microsoft Edge

Microsoft Edge bevat [bekende problemen](https://go.microsoft.com/fwlink/?linkid=2140608) die zijn gerelateerd aan beveiligingszones en van invloed kunnen zijn op hoe Azure gebruikers zich aanmelden bij het Windows-Beheercentrum. Als u problemen ondervindt bij het gebruiken van Azure-functies met Microsoft Edge, voert u de volgende stappen uit:

1. Selecteer in het **Start** menu de **optie Internet opties** en selecteer deze.
2. Ga in het dialoogvenster **Internet eigenschappen** naar het tabblad **beveiliging** .
3. Selecteer de zone **vertrouwde websites** en selecteer vervolgens de knop **sites** .
4. In het dialoogvenster **vertrouwde websites** voegt u de gateway-URL en [https://login.microsoftonline.com](https://login.microsoftonline.com) en [https://login.live.com](https://login.live.com) selecteert u vervolgens **sluiten**.
5. Ga naar het tabblad **Privacy** in het dialoogvenster **Internet eigenschappen** .
6. Selecteer in de sectie **pop-upblokkering** de optie **instellingen**. In het dialoogvenster dat wordt geopend, voegt u de gateway-URL en [https://login.microsoftonline.com](https://login.microsoftonline.com) en [https://login.live.com](https://login.live.com) selecteert u vervolgens **sluiten**.
