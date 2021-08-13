---
title: Verwijder permanent een site in SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944306"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Verwijder permanent een site in SharePoint

Om een URL van een verwijderde site opnieuw te gebruiken (om een site opnieuw te maken) of om een site permanent te verwijderen omdat deze niet langer in gebruik is, kunt u **Permanent verwijderen** gebruiken in het nieuwe SharePoint Admin Center. 

1. Ga naar de [ pagina met verwijderde sites van het nieuwe SharePoint-beheercentrum ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) en log in met een account dat beheerdersrechten heeft voor uw organisatie. 

2. Selecteer in de linkerkolom een site. 

3. Klik op **Permanent verwijderen**. 

**Opmerking**: Groepsgebonden sites kunnen niet permanent worden verwijderd uit het nieuwe SharePoint Admin Center. In plaats daarvan moet [ Remove-SPODeletedSite ](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) worden gebruikt.  

Zie [ Een site definitief verwijderen ](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) voor meer informatie. 
