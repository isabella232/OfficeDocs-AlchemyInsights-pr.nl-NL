---
title: Fix 0x8004de40 fout in OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755843"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 fout in OneDrive

Als u een fout 0x8004de40 met OneDrive ontvangt:

- Start de betrokken computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.
- Als het probleem niet wordt opgelost door een reboot, loskoppelen en opnieuw deelnemen aan uw apparaat van Azure AD. 

**Opmerking**: u moet zich op uw bedrijfsnetwerk bevinden tijdens het uitvoeren van deze stappen. Voer deze stappen niet uit wanneer u geen verbinding maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen). 

- Open een opdrachtprompt met verhoogde bevoegdheid. 
- Als u wilt een opdrachtprompt met verhoogde bevoegdheid openen, klikt u op-Start, Klik **met**de rechtermuisknop op **opdrachtprompt**en klik vervolgens op **als administrator uitvoeren**.
- Typ *dsregcmd/Leave* en druk op **Enter**.
- Als u klaar is, typt u *dsregcmd/join kunnen* en drukt **u op ENTER**.
- Wanneer u klaar is, sluit u de opdrachtprompt.
- Start de computer opnieuw op en meld u aan bij OneDrive.