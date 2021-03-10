---
title: Problemen met de installatie van MDATP op een Mac oplossen
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693349"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Problemen met de installatie van MDATP op een Mac oplossen

Als de handmatige installatie mislukt, **wordt op de pagina** Samenvatting van de installatiewizard de volgende fout weergegeven:

'Er is een fout opgetreden tijdens de installatie. Er is een fout opgetreden waardoor de installatie is mislukt. Neem contact op met de softwarefabrikant voor hulp.'

Voor MDM-implementaties wordt op de pagina ook een algemene installatiefout weergegeven.

Hoewel er geen exacte fouten worden weergegeven aan eindgebruikers, wordt er wel een logboekbestand met de voortgang van de installatie bijgeslagen in **/Library/Logs/Microsoft/mdatp/install.log.** Elke installatiesessie wordt toegevoegd aan dit logboekbestand. Als u alleen de laatste installatiesessie wilt uitvoeren, gebruikt u `sed` .

Zie Installatieproblemen oplossen [voor Microsoft Defender ATP voor Mac voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144615)
