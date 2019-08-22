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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525054"
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