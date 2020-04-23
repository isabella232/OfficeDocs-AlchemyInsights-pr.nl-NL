---
title: 0x8004de40-fout oplossen in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716023"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40-fout oplossen in OneDrive

Als u een fout van 0x8004de40 met OneDrive ontvangt:

- Start de betreffende computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.
- Als een reboot het probleem niet oplost, sluit u de join en sluit u uw apparaat opnieuw aan vanuit Azure AD. 

**Opmerking:** U moet zich tijdens het uitvoeren van deze stappen in uw bedrijfsnetwerk bevinden. Voer deze stappen niet uit wanneer u geen verbinding maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen). 

- Open een opdrachtprompt met verhoogde bevoegdheid. 
- Als u een opdrachtprompt met verhoogde bevoegdheid wilt openen, klikt u op - **Start**, klikt u met de rechtermuisknop op **Opdrachtprompt**en klikt u vervolgens op **Uitvoeren als beheerder**.
- Typ *dsregcmd /leave* en druk op **Enter**.
- Als u klaar bent, typt u *dsregcmd /join* en drukt u op **Enter**.
- Als u klaar bent, sluit u de opdrachtprompt.
- Start de computer opnieuw op en meld u aan bij OneDrive.