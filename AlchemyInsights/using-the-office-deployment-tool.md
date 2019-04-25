---
title: Met behulp van de Office Deployment Tool
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423178"
---
# <a name="using-the-office-deployment-tool-odt"></a>Met behulp van de Office Deployment Tool (ODT)

Met de Office Deployment Tool (ODT) kunt u het implementeren van Office 365-versies van Office. De Office Deployment Tool (setup.exe) wordt uitgevoerd vanaf de opdrachtregel en een XML-configuratiebestand gebruikt om te bepalen welke instellingen toe te passen bij het implementeren van Office.
  
1. De nieuwste versie van de Office Deployment Tool downloaden van het [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Gebruik de [Office Customization Tool (OCT)](https://config.office.com) Selecteer uw voorkeuren voor de implementatie en het XML-configuratiebestand maken. Het configuratiebestand exporteren en lokaal op de map waarin zich de setup.exe bevindt. 
    
    **Opmerking:** Malformatted configuratiebestanden of vaak verschuldigd aan onjuist geconfigureerde problemen Office-installatie. Om deze problemen te vermijden, is het raadzaam gebruik te maken van de Office Customization Tool voor het maken van het configuratiebestand. U kunt ook bestaande configuratiebestanden importeren in de Office Customization Tool. 
    
3. Overschakelen naar de locatie waar de setup.exe bevindt zich vanaf een opdrachtprompt en de Office Deployment Tool uitvoeren in de downloadmodus en geef het configuratiebestand dat u zojuist hebt opgeslagen. In dit voorbeeld wordt het configuratiebestand met de naam Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. De Office Deployment Tool uitvoeren in modus configureren en geeft u het configuratiebestand.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Opmerking:** U moet deze stap uitvoeren vanaf de clientcomputer waarop u Office wilt installeren en hebt u lokale beheerdersmachtigingen op de computer. 
    
Zie voor meer informatie over het gebruik van de Office Deployment Tool voor uw Office 365 ProPlus implementatiescenario's, [overzicht van de Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Zie voor meer informatie over het gebruik van de Office Customization Tool [-overzicht van de Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

