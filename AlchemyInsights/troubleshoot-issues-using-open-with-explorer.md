---
title: Problemen oplossen met openen met Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659053"
---
# <a name="fix-problems-with-open-with-explorer"></a>Problemen oplossen met openen met Explorer

Veelvoorkomende problemen met het openen van een documentbibliotheek in SharePoint of OneDrive oplossen met de opdracht **openen met Explorer** : 
  
- Internet Explorer 10 of Internet Explorer 11 gebruiken. **Openen met Explorer** is niet compatibel met Microsoft Edge, Google Chrome, Firefox en andere. **Openen met Explorer** is uitgeschakeld in alle browsers, met uitzondering van Internet Explorer. 
    
- **Openen met Explorer** is niet beschikbaar in de moderne ervaring voor SharePoint-bibliotheken. Gebruik in plaats hiervan **weergave in Verkenner** . Selecteer weergave **Opties** \> **weergeven in Verkenner**. Weergeven in bestandenverkenner is niet compatibel met Microsoft Edge, Google Chrome, Firefox en andere. **Weergeven in de Verkenner** in alleen beschikbaar in Internet Explorer. 
    
- Zorg ervoor dat de client service wordt uitgevoerd. Typ in het vak Windows Search de tekst run, selecteer de bureaublad-app uitvoeren, typ services. msc en druk op ENTER. Schuif omlaag naar de WebClient service en zorg ervoor dat in de kolom **status** de waarde ' uitvoeren ' wordt weergegeven. Als dit niet het geval is, dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**. (Mogelijk moet u eerst de service inschakelen door **handmatig** of **automatisch** in het vak **Opstarttype** te selecteren.) 
    
> [!NOTE]
> Het openen van een bibliotheek in Verkenner is handig als u meerdere bestanden en mappen wilt kopiëren of verplaatsen, maar als u regelmatig wilt werken in de bibliotheek, is het raadzaam om deze te synchroniseren. Zie [openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor informatie over het oplossen van problemen met openen in de Verkenner. Voor informatie over het instellen van synchronisatie raadpleegt u [SharePoint-bestanden synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Zie het artikel [hoe u met de opdracht ' openen met Explorer ' problemen oplost in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) voor meer informatie. 
  

