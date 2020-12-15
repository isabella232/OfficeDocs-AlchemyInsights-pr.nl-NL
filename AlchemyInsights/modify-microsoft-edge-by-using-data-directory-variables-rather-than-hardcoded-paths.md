---
title: Microsoft Edge aanpassen met behulp van gegevenslabel variabelen in plaats van hardcoded paden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677332"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Microsoft Edge aanpassen met behulp van gegevenslabel variabelen in plaats van hardcoded paden

Als u in Windows bijvoorbeeld de profielgegevens onder de lokale toepassingsgegevens van een gebruiker wilt opslaan in plaats van in de standaardlocatie, stelt u het **UserDataDir** -beleid in op **$ {local_app_data} \Edge\Profile**. 

Zie [Microsoft Edge User datadirectory-variabelen maken](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)voor meer informatie.