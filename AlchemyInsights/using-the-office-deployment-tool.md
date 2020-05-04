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
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010852"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="d66ea-102">Het Office Deployment Tool (ODT) gebruiken</span><span class="sxs-lookup"><span data-stu-id="d66ea-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d66ea-103">U gebruikt de ODT (Office Deployment Tool) om Office 365-versies van Office te implementeren.</span><span class="sxs-lookup"><span data-stu-id="d66ea-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="d66ea-104">Het Office Deployment Tool (setup.exe) wordt uitgevoerd vanaf de opdrachtregel en gebruikt een configuratie-XML-bestand om te bepalen welke instellingen u moet toepassen bij het implementeren van Office.</span><span class="sxs-lookup"><span data-stu-id="d66ea-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="d66ea-105">Download de nieuwste versie van het Office Deployment Tool in het [Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="d66ea-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="d66ea-106">Gebruik het [Office Customization Tool (OCT)](https://config.office.com) om uw implementatievoorkeuren te selecteren en het XML-configuratiebestand te maken.</span><span class="sxs-lookup"><span data-stu-id="d66ea-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="d66ea-107">Exporteer het configuratiebestand en plaats het lokaal op dezelfde map waar de setup.exe zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="d66ea-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="d66ea-108">**Let op:** Problemen met de installatie van Office komen vaak voor als gevolg van verkeerd geconfigureerde of verkeerd ingemaakte configuratiebestanden.</span><span class="sxs-lookup"><span data-stu-id="d66ea-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="d66ea-109">Om dergelijke problemen te voorkomen, raden we u aan het Office Customization Tool te gebruiken om het configuratiebestand te maken.</span><span class="sxs-lookup"><span data-stu-id="d66ea-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="d66ea-110">U ook bestaande configuratiebestanden importeren in het Office Customization Tool.</span><span class="sxs-lookup"><span data-stu-id="d66ea-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="d66ea-111">Ga vanuit een opdrachtprompt met verhoogde bevoegdheid over naar de locatie waar setup.exe zich bevindt en voer het Office Deployment Tool uit in de downloadmodus en geef het configuratiebestand op dat u zojuist hebt opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="d66ea-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="d66ea-112">In dit voorbeeld wordt het configuratiebestand Configuration.xml genoemd:</span><span class="sxs-lookup"><span data-stu-id="d66ea-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="d66ea-113">Voer het Office Deployment Tool uit in de configureermodus en geef het configuratiebestand op.</span><span class="sxs-lookup"><span data-stu-id="d66ea-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="d66ea-114">**Let op:** U moet deze stap uitvoeren vanaf de clientcomputer waarop u Office wilt installeren en u moet lokale beheerdersmachtigingen op die computer hebben.</span><span class="sxs-lookup"><span data-stu-id="d66ea-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="d66ea-115">Zie [Overzicht van het Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)voor meer informatie over het gebruik van Office Deployment Tool voor uw Microsoft 365 Apps voor bedrijfsimplementatiescenario's.</span><span class="sxs-lookup"><span data-stu-id="d66ea-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="d66ea-116">Zie [Overzicht van het Office-aanpassingsprogramma](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)voor meer informatie over het gebruik van het Office-aanpassingsprogramma .</span><span class="sxs-lookup"><span data-stu-id="d66ea-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
