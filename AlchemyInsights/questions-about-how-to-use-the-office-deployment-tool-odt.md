---
title: Vragen over het gebruik van de ODT (Office Deployment Tool)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010727"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="5f502-102">Vragen over het gebruik van de ODT (Office Deployment Tool)</span><span class="sxs-lookup"><span data-stu-id="5f502-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5f502-103">Download het Office Deployment Tool in het [Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="5f502-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="5f502-104">Nadat u het bestand hebt gedownload, voert u het uitvoerbare bestand zelf uit, dat het uitvoerbare Office Deployment Tool (setup.exe) en een voorbeeldconfiguratiebestand (configuration.xml) bevat.</span><span class="sxs-lookup"><span data-stu-id="5f502-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="5f502-105">**Ga als u Microsoft 365 Apps voor bedrijfsproducten uitof verwijderen van clientcomputers:**</span><span class="sxs-lookup"><span data-stu-id="5f502-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="5f502-106">Wanneer u Microsoft 365 Apps voor bedrijven installeert, u specifieke producten uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="5f502-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="5f502-107">Volg hiervoor de stappen voor het installeren van Office met de ODT, maar neem het element ExcludeApp op in uw configuratiebestand.</span><span class="sxs-lookup"><span data-stu-id="5f502-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="5f502-108">In dit configuratiebestand worden bijvoorbeeld alle Microsoft 365-apps voor bedrijfsproducten geïnstalleerd, behalve Publisher:</span><span class="sxs-lookup"><span data-stu-id="5f502-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="5f502-109">Overzicht van het hulpprogramma voor office-implementatie</span><span class="sxs-lookup"><span data-stu-id="5f502-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

