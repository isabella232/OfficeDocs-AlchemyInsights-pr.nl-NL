---
title: Met behulp van de Office Deployment Tool
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29465095"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="74bb5-102">Met behulp van de Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="74bb5-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="74bb5-p101">Met de Office Deployment Tool (ODT) kunt u het implementeren van Office 365-versies van Office. De Office Deployment Tool (setup.exe) wordt uitgevoerd vanaf de opdrachtregel en een XML-configuratiebestand gebruikt om te bepalen welke instellingen toe te passen bij het implementeren van Office.</span><span class="sxs-lookup"><span data-stu-id="74bb5-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="74bb5-105">De nieuwste versie van de Office Deployment Tool downloaden van het [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="74bb5-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="74bb5-p102">Gebruik de [Office Customization Tool (OCT)](https://config.office.com) Selecteer uw voorkeuren voor de implementatie en het XML-configuratiebestand maken. Het configuratiebestand exporteren en lokaal op de map waarin zich de setup.exe bevindt.</span><span class="sxs-lookup"><span data-stu-id="74bb5-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="74bb5-p103">**Opmerking:** Malformatted configuratiebestanden of vaak verschuldigd aan onjuist geconfigureerde problemen Office-installatie. Om deze problemen te vermijden, is het raadzaam gebruik te maken van de Office Customization Tool voor het maken van het configuratiebestand. U kunt ook bestaande configuratiebestanden importeren in de Office Customization Tool.</span><span class="sxs-lookup"><span data-stu-id="74bb5-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="74bb5-p104">Overschakelen naar de locatie waar de setup.exe bevindt zich vanaf een opdrachtprompt en de Office Deployment Tool uitvoeren in de downloadmodus en geef het configuratiebestand dat u zojuist hebt opgeslagen. In dit voorbeeld wordt het configuratiebestand met de naam Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="74bb5-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="74bb5-113">De Office Deployment Tool uitvoeren in modus configureren en geeft u het configuratiebestand.</span><span class="sxs-lookup"><span data-stu-id="74bb5-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="74bb5-114">**Opmerking:** U moet deze stap uitvoeren vanaf de clientcomputer waarop u Office wilt installeren en hebt u lokale beheerdersmachtigingen op de computer.</span><span class="sxs-lookup"><span data-stu-id="74bb5-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="74bb5-p105">Zie voor meer informatie over het gebruik van de Office Deployment Tool voor uw Office 365 ProPlus implementatiescenario's, [overzicht van de Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Zie voor meer informatie over het gebruik van de Office Customization Tool [-overzicht van de Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="74bb5-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

