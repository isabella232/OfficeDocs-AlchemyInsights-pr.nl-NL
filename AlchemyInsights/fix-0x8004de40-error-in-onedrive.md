---
title: Fout 0x8004de40 in OneDrive oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649743"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fout 0x8004de40 in OneDrive oplossen

Als u Windows 7 gebruikt en deze fout ontvangt, kunt u bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)in te stellen als standaardveilige protocollen in WinHTTP in Windows.

Als u Windows 10 gebruikt en u een foutmelding 0x8004de40 OneDrive:

- Start de betreffende computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.
- Als het probleem niet wordt opgelost door opnieuw op te starten, ontvoegt u het apparaat en maakt u opnieuw gebruik van Azure AD. 

**Opmerking:** u moet in uw bedrijfsnetwerk zijn terwijl u deze stappen voert. Voer deze stappen niet uit wanneer u niet bent verbonden met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen). 

1. Open een opdrachtprompt met verhoogde opdracht door **Start** te selecteren, met de rechtermuisknop op **Opdrachtprompt** te klikken en vervolgens **Uitvoeren als beheerder te selecteren.**

1. Typ *dsregcmd /leave* en druk op **Enter.**

1. Als u klaar is, *typt u dsregcmd /join en drukt* u op **Enter.**

1. Als u klaar is, sluit u de opdrachtprompt.

1. Start de computer opnieuw op en meld u aan bij OneDrive.