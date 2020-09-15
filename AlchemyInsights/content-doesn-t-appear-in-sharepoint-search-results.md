---
title: Inhoud wordt niet weergegeven in de zoekresultaten van SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713125"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Inhoud wordt niet weergegeven in de zoekresultaten van SharePoint

Volg deze stappen voor probleemoplossing wanneer verwachte inhoud niet in de zoekresultaten wordt weergegeven:
  
1. Controleer of de **site** die de verwachte inhoud bevat, is ingesteld op toestaan dat inhoud wordt weergegeven in zoekresultaten. Volg de stappen in de [inhoud van een site weergeven in zoekresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Controleer of de **lijst** of **bibliotheek** die de verwachte inhoud bevat, is ingesteld op toestaan dat inhoud wordt weergegeven in zoekresultaten. Volg de stappen in [inhoud van lijsten of bibliotheken weergeven in zoekresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Controleer of de pagina, het document of de aangepaste pagina-indeling is gepubliceerd als een **primaire versie.** Voer stap 3 in [de zoekfunctie retourneert niet alle resultaten in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Controleer of de gebruiker **gemachtigd** is om de inhoud weer te geven. Volg de stappen in [machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Als het zoekschema is gewijzigd door een nieuwe beheerde eigenschap toe te voegen, of door een beheerde eigenschap te bewerken, of door een beheerde eigenschap te verwijderen, moet u een verkenning en een nieuwe index aanvragen. **Indexeer** de inhoud opnieuw door de stappen te volgen in het [handmatig verkennen en opnieuw indexeren van een site, bibliotheek of lijst](https://docs.microsoft.com/sharepoint/crawl-site-content). Het kan enige tijd duren voordat u de resultaten opnieuw controleert.

Zie voor meer informatie [inhoud op een site inschakelen om te kunnen zoeken](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
