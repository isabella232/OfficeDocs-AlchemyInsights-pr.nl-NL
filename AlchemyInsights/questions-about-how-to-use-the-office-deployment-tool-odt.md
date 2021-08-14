---
title: Vragen over het gebruik van het Office Implementatieprogramma (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959678"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van het Office Implementatieprogramma (ODT)

Download het Office implementatieprogramma van [het Microsoft Downloadcentrum.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Nadat u het bestand hebt gedownload, voert u het zelfuitvoerbare uitvoerbare bestand uit, dat het uitvoerbare Office-implementatieprogramma (setup.exe) en een voorbeeldconfiguratiebestand (configuration.xml) bevat.
  
 **Als u producten van clientcomputers wilt uitsluiten Microsoft 365-apps voor ondernemingen verwijderen:**
  
Wanneer u Microsoft 365-apps voor ondernemingen, kunt u specifieke producten uitsluiten. Volg de stappen voor het installeren van Office odt, maar neem het element ExcludeApp op in het configuratiebestand. In dit configuratiebestand worden bijvoorbeeld alle Microsoft 365-apps voor ondernemingen geïnstalleerd, behalve Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van het Office implementatieprogramma](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

