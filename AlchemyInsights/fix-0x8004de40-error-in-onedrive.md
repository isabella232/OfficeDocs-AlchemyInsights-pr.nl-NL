---
title: 0x8004de40 fout in OneDrive oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745125"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40 fout in OneDrive oplossen

Als u een 0x8004de40-fout ontvangt met OneDrive:

- Start de desbetreffende computer opnieuw op terwijl u verbinding hebt met uw Acitve-Directory domein.
- Als het probleem niet is verholpen nadat u de computer opnieuw hebt opgestart, ontkoppelt u uw apparaat en voegt u het opnieuw aan via Azure AD. 

**Opmerking**: u moet zich op uw bedrijfsnetwerk bevinden wanneer u deze stappen uitvoert. Voer deze stappen uit als u geen verbinding kunt maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens reis). 

- Open een opdrachtprompt met verhoogde bevoegdheid. 
- Als u een opdrachtprompt met verhoogde bevoegdheid wilt openen, klikt u op **Start**, klikt u met de rechtermuisknop op **opdrachtprompt**en klikt u vervolgens op **als administrator uitvoeren**.
- Typ *dsregcmd/Leave* en druk op **Enter**.
- Wanneer u klaar bent, typt u *dsregcmd/join* en drukt u op **Enter**.
- Wanneer u klaar bent, sluit u de opdrachtprompt.
- Start de computer opnieuw op en meld u aan bij OneDrive.