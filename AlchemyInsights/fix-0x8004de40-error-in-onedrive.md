---
title: 0x8004de40-fout oplossen in OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133972"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40-fout oplossen in OneDrive

Als er een fout 0x8004de40 met OneDrive:

- Start opnieuw op de desbetreffende computer terwijl verbonden met uw Acitve Directory-domein.
- Als opnieuw opstarten het probleem niet is verholpen, loskoppelen en weer lid worden van het apparaat uit Azure Active Directory. 

**Opmerking**: U moet op uw bedrijfsnetwerk worden tijdens het uitvoeren van deze stappen. Niet deze stappen niet uitvoeren wanneer u geen verbinding kunnen maken met uw bedrijfsinfrastructuur (bijvoorbeeld wanneer u onderweg bent). 

- Open een opdrachtprompt. 
- U opent een opdrachtprompt, op - **Start**, klik met de rechtermuisknop op **opdrachtprompt**en klik vervolgens op **Als administrator uitvoeren**.
- *Dsregcmd /leave* en druk op **Enter**.
- Als alles klaar is, *dsregcmd, /join* en druk op **Enter**.
- Als alles klaar is, sluit u de opdrachtprompt.
- Start de computer opnieuw op en meld u aan bij OneDrive.