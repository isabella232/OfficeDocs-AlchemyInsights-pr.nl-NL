---
title: Vragen over het gebruik van het Office-implementatieprogramma (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774886"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van het Office-implementatieprogramma (ODT)

Download het Office-implementatieprogramma in het [Microsoft Download centrum](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nadat u het bestand hebt gedownload, voert u het zelfuitpakkende uitvoerbare bestand uit, dat het uitvoerbare Office-implementatieprogramma (setup.exe) en een voorbeeld van een configuratiebestand (configuration.xml) bevat.
  
 **Microsoft 365-apps voor Enterprise-producten uitsluiten of verwijderen van clientcomputers:**
  
Wanneer u Microsoft 365-apps voor Enterprise installeert, kunt u bepaalde producten uitsluiten. Hiertoe volgt u de stappen voor het installeren van Office met behulp van ODT, maar neemt u het element ExcludeApp op in uw configuratiebestand. Dit configuratiebestand installeert bijvoorbeeld alle Microsoft 365-apps voor Enterprise-producten, met uitzondering van Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van het Office-implementatieprogramma](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

