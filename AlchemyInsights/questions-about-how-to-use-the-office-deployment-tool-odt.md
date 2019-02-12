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
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925339"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vragen over het gebruik van de Office Deployment Tool (ODT)

De Office Deployment Tool downloaden van het [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Voer het zelfuitpakkende uitvoerbare bestand waarin de Office Deployment Tool uitvoerbaar bestand (setup.exe) en een voorbeeld configuratiebestand (configuration.xml) downloaden van het bestand.
  
 **Sluiten of verwijderen van Office 365 ProPlus producten van clientcomputers:**
  
Bij het installeren van Office 365 ProPlus, kunt u bepaalde producten uitsluiten. Hiertoe volgt u de stappen voor het installeren van Office met de ODT, maar het ExcludeApp-element opnemen in uw configuratiebestand. Dit configuratiebestand worden geïnstalleerd, bijvoorbeeld Office 365 ProPlus producten, met uitzondering van Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overzicht van de Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

