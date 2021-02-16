---
title: Apparaat inschakelen
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256757"
---
# <a name="enable-device"></a>Apparaat inschakelen

**Het apparaat inschakelen via de PowerShell-opdracht**

Voer de volgende opdrachten uit:

- Apparaatobject op te halen: `Get-MsolDevice -Name <Name>`
- Apparaat inschakelen: `Enable-MsolDevice -DeviceId <DeviceId>`

Zie Hybride join configureren voor meer informatie over het configureren van hybride join voor [beheerde domeinen.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
