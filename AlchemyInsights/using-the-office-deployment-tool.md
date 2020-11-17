---
title: Werken met het Office-implementatieprogramma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085827"
---
# <a name="using-the-office-deployment-tool-odt"></a>Het Office-implementatieprogramma (ODT) gebruiken

U gebruikt het Office-implementatieprogramma (ODT) om Office 365-versies van Office te implementeren. Het Office-implementatieprogramma (setupodt.exe) wordt uitgevoerd vanaf de opdrachtregel en gebruikt een XML-configuratiebestand om te bepalen welke instellingen bij de implementatie van Office gelden.
  
1. Download de meest recente versie van het Office-implementatieprogramma in het [Microsoft Download centrum](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Gebruik het [Office Customization Tool (OCT)](https://config.office.com) om uw implementatie voorkeuren te selecteren en maak het XML-configuratiebestand. Exporteer het configuratiebestand en zet dit lokaal op de map waarin het setupodt.exe zich bevindt.

    **Opmerking:** Problemen met de installatie van Office zijn vaak veroorzaakt door verkeerd geconfigureerde of malformatted configuratiebestanden. Om dit probleem te voorkomen, raden we u aan om het Office Customization Tool te gebruiken voor het maken van het configuratiebestand. U kunt ook bestaande configuratiebestanden importeren in het hulpprogramma voor aanpassing van Office.

3. Vanaf een opdrachtprompt met verhoogde bevoegdheid gaat u naar de locatie waar setupodt.exe zich bevindt, voert u het Office-implementatieprogramma in de downloadmodus uit en geeft u het configuratiebestand op dat u zojuist hebt opgeslagen. In dit voorbeeld heeft het configuratiebestand de naam Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Voer het Office-implementatieprogramma uit in de modus configureren en geef het configuratiebestand op.

```setupodt.exe /configure Configuration.xml```

**Opmerking:** U moet deze stap uitvoeren op de clientcomputer waarop u Office wilt installeren en moet de machtigingen voor lokale beheerders op de computer zijn geïnstalleerd.

Voor meer informatie over het gebruik van het Office-implementatieprogramma voor uw Microsoft 365-apps voor Enterprise-implementatiescenario's, raadpleegt u [overzicht van het Office-implementatieprogramma](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Zie voor meer informatie over het gebruik van het Office Customization Tool [overzicht van het Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
