---
title: Vragen over het gebruik van de Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553535"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van de Office Deployment Tool (ODT)

Download het Office Deployment Tool van het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nadat u het bestand hebt gedownload, voert u het zelfuitpakkende uitvoerbare bestand uit dat het uitvoerbare Office-hulpprogramma (Setup. exe) en een voorbeeldconfiguratiebestand (Configuration. XML) bevat.
  
 **Om Office 365 ProPlus-producten van clientcomputers uit te sluiten of te verwijderen:**
  
Bij de installatie van Office 365 ProPlus u specifieke producten uitsluiten. Om dit te doen, volgt u de stappen voor het installeren van Office met de ODT, maar het element ExcludeApp in uw configuratiebestand opnemen. Met dit configuratiebestand worden bijvoorbeeld alle Office 365 ProPlus-producten geïnstalleerd, behalve Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van het Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

