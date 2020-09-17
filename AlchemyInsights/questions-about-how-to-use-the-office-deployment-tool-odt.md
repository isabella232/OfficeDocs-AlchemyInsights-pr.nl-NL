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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="dd709-102">Vragen over het gebruik van het Office-implementatieprogramma (ODT)</span><span class="sxs-lookup"><span data-stu-id="dd709-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="dd709-103">Download het Office-implementatieprogramma in het [Microsoft Download centrum](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="dd709-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="dd709-104">Nadat u het bestand hebt gedownload, voert u het zelfuitpakkende uitvoerbare bestand uit, dat het uitvoerbare Office-implementatieprogramma (setup.exe) en een voorbeeld van een configuratiebestand (configuration.xml) bevat.</span><span class="sxs-lookup"><span data-stu-id="dd709-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="dd709-105">**Microsoft 365-apps voor Enterprise-producten uitsluiten of verwijderen van clientcomputers:**</span><span class="sxs-lookup"><span data-stu-id="dd709-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="dd709-106">Wanneer u Microsoft 365-apps voor Enterprise installeert, kunt u bepaalde producten uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="dd709-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="dd709-107">Hiertoe volgt u de stappen voor het installeren van Office met behulp van ODT, maar neemt u het element ExcludeApp op in uw configuratiebestand.</span><span class="sxs-lookup"><span data-stu-id="dd709-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="dd709-108">Dit configuratiebestand installeert bijvoorbeeld alle Microsoft 365-apps voor Enterprise-producten, met uitzondering van Publisher:</span><span class="sxs-lookup"><span data-stu-id="dd709-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="dd709-109">Overzicht van het Office-implementatieprogramma</span><span class="sxs-lookup"><span data-stu-id="dd709-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

