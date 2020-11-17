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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="1af4c-102">Het Office-implementatieprogramma (ODT) gebruiken</span><span class="sxs-lookup"><span data-stu-id="1af4c-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="1af4c-103">U gebruikt het Office-implementatieprogramma (ODT) om Office 365-versies van Office te implementeren.</span><span class="sxs-lookup"><span data-stu-id="1af4c-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="1af4c-104">Het Office-implementatieprogramma (setupodt.exe) wordt uitgevoerd vanaf de opdrachtregel en gebruikt een XML-configuratiebestand om te bepalen welke instellingen bij de implementatie van Office gelden.</span><span class="sxs-lookup"><span data-stu-id="1af4c-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="1af4c-105">Download de meest recente versie van het Office-implementatieprogramma in het [Microsoft Download centrum](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="1af4c-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="1af4c-106">Gebruik het [Office Customization Tool (OCT)](https://config.office.com) om uw implementatie voorkeuren te selecteren en maak het XML-configuratiebestand.</span><span class="sxs-lookup"><span data-stu-id="1af4c-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="1af4c-107">Exporteer het configuratiebestand en zet dit lokaal op de map waarin het setupodt.exe zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="1af4c-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="1af4c-108">**Opmerking:** Problemen met de installatie van Office zijn vaak veroorzaakt door verkeerd geconfigureerde of malformatted configuratiebestanden.</span><span class="sxs-lookup"><span data-stu-id="1af4c-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="1af4c-109">Om dit probleem te voorkomen, raden we u aan om het Office Customization Tool te gebruiken voor het maken van het configuratiebestand.</span><span class="sxs-lookup"><span data-stu-id="1af4c-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="1af4c-110">U kunt ook bestaande configuratiebestanden importeren in het hulpprogramma voor aanpassing van Office.</span><span class="sxs-lookup"><span data-stu-id="1af4c-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="1af4c-111">Vanaf een opdrachtprompt met verhoogde bevoegdheid gaat u naar de locatie waar setupodt.exe zich bevindt, voert u het Office-implementatieprogramma in de downloadmodus uit en geeft u het configuratiebestand op dat u zojuist hebt opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="1af4c-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="1af4c-112">In dit voorbeeld heeft het configuratiebestand de naam Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="1af4c-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="1af4c-113">4. Voer het Office-implementatieprogramma uit in de modus configureren en geef het configuratiebestand op.</span><span class="sxs-lookup"><span data-stu-id="1af4c-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="1af4c-114">**Opmerking:** U moet deze stap uitvoeren op de clientcomputer waarop u Office wilt installeren en moet de machtigingen voor lokale beheerders op de computer zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="1af4c-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="1af4c-115">Voor meer informatie over het gebruik van het Office-implementatieprogramma voor uw Microsoft 365-apps voor Enterprise-implementatiescenario's, raadpleegt u [overzicht van het Office-implementatieprogramma](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="1af4c-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="1af4c-116">Zie voor meer informatie over het gebruik van het Office Customization Tool [overzicht van het Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="1af4c-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
