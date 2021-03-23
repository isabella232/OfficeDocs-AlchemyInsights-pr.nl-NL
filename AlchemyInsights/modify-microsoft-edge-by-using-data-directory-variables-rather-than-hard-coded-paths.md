---
title: Microsoft Edge wijzigen met behulp van gegevensmapvariabelen in plaats van hardcoded paden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035282"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Microsoft Edge wijzigen met behulp van gegevensmapvariabelen in plaats van hardcoded paden

Als u bijvoorbeeld in Windows de profielgegevens wilt opslaan onder de lokale toepassingsgegevens van een gebruiker in plaats van op de standaardlocatie, stelt u het *UserDataDir-beleid* in op **${local_app_data}\Edge\Profile.**

Zie Microsoft [Edge-gebruikersgegevensmapvariabelen maken voor meer informatie.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)