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
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698053"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van de ODT (Office Deployment Tool)

Download het Office Deployment Tool in het [Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Nadat u het bestand hebt gedownload, voert u het uitvoerbare bestand zelf uit, dat het uitvoerbare Office Deployment Tool (setup.exe) en een voorbeeldconfiguratiebestand (configuration.xml) bevat.
  
 **Ga als u Microsoft 365 Apps voor bedrijfsproducten uitof verwijderen van clientcomputers:**
  
Wanneer u Microsoft 365 Apps voor bedrijven installeert, u specifieke producten uitsluiten. Volg hiervoor de stappen voor het installeren van Office met de ODT, maar neem het element ExcludeApp op in uw configuratiebestand. In dit configuratiebestand worden bijvoorbeeld alle Microsoft 365-apps voor bedrijfsproducten geïnstalleerd, behalve Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van het hulpprogramma voor office-implementatie](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

