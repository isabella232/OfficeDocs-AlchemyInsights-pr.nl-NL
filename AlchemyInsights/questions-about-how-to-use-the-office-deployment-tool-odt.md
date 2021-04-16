---
title: Vragen over het gebruik van het Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790327"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van het Office Deployment Tool (ODT)

Download het Office-implementatieprogramma vanuit het [Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Nadat u het bestand hebt gedownload, voert u het zelfuitvoerbare uitvoerbare bestand uit, dat het uitvoerbare Office-implementatieprogramma (setup.exe) en een voorbeeldconfiguratiebestand (configuration.xml).
  
 **Microsoft 365 Apps voor ondernemingsproducten uitsluiten of verwijderen van clientcomputers:**
  
Wanneer u Microsoft 365 Apps voor ondernemingen installeert, kunt u specifieke producten uitsluiten. Als u dit wilt doen, volgt u de stappen voor het installeren van Office met de ODT, maar neemt u het element ExcludeApp op in het configuratiebestand. In dit configuratiebestand worden bijvoorbeeld alle Microsoft 365-apps voor ondernemingsproducten, behalve Publisher, geïnstalleerd:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van het Office-implementatieprogramma](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

