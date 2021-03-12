---
title: Problemen met MDATP-installatie op een Mac oplossen
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744658"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Problemen met MDATP-installatie op een Mac oplossen

Als handmatige installatie mislukt, wordt op **de pagina** Overzicht van de installatiewizard de volgende fout weergegeven:

'Er is een fout opgetreden tijdens de installatie. Bij het installatieprogramma is een fout opgetreden waardoor de installatie is mislukt. Neem contact op met de softwarefabrikant voor hulp.

Voor MDM-implementaties wordt op de pagina ook een algemene installatiefout weergegeven.

Hoewel er geen exacte fouten worden weergegeven voor eindgebruikers, bewaren we een logboekbestand met de voortgang van de installatie, in **/Library/Logs/Microsoft/mdatp/install.log.** Elke installatiesessie wordt toegevoegd aan dit logboekbestand. Als u alleen de laatste installatiesessie wilt uitvoeren, gebruikt u `sed` .

Zie Installatieproblemen oplossen [voor Microsoft Defender ATP voor Mac voor](https://go.microsoft.com/fwlink/?linkid=2144615)meer informatie.
