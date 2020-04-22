---
title: Het hulpprogramma voor Office-implementatie gebruiken
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726243"
---
# <a name="using-the-office-deployment-tool-odt"></a>Het Office Deployment Tool (ODT) gebruiken

U gebruikt de ODT (Office Deployment Tool) om Office 365-versies van Office te implementeren. Het Office Deployment Tool (setup.exe) wordt uitgevoerd vanaf de opdrachtregel en gebruikt een configuratie-XML-bestand om te bepalen welke instellingen u moet toepassen bij het implementeren van Office.
  
1. Download de nieuwste versie van het Office Deployment Tool in het [Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Gebruik het [Office Customization Tool (OCT)](https://config.office.com) om uw implementatievoorkeuren te selecteren en het XML-configuratiebestand te maken. Exporteer het configuratiebestand en plaats het lokaal op dezelfde map waar de setup.exe zich bevindt.

    **Let op:** Problemen met de installatie van Office komen vaak voor als gevolg van verkeerd geconfigureerde of verkeerd ingemaakte configuratiebestanden. Om dergelijke problemen te voorkomen, raden we u aan het Office Customization Tool te gebruiken om het configuratiebestand te maken. U ook bestaande configuratiebestanden importeren in het Office Customization Tool.

3. Ga vanuit een opdrachtprompt met verhoogde bevoegdheid over naar de locatie waar setup.exe zich bevindt en voer het Office Deployment Tool uit in de downloadmodus en geef het configuratiebestand op dat u zojuist hebt opgeslagen. In dit voorbeeld wordt het configuratiebestand Configuration.xml genoemd:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Voer het Office Deployment Tool uit in de configureermodus en geef het configuratiebestand op.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Let op:** U moet deze stap uitvoeren vanaf de clientcomputer waarop u Office wilt installeren en u moet lokale beheerdersmachtigingen op die computer hebben.

Zie [Overzicht van het Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)voor meer informatie over het gebruik van Office Deployment Tool voor uw Microsoft 365 Apps voor bedrijfsimplementatiescenario's. Zie [Overzicht van het Office-aanpassingsprogramma](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)voor meer informatie over het gebruik van het Office-aanpassingsprogramma .
