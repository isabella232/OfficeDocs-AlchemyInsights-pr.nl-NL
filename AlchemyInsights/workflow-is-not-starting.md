---
title: Werkstroom wordt niet gestart
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794762"
---
# <a name="workflow-is-not-starting"></a>Werkstroom wordt niet gestart

- Werkstromen van SharePoint 2010 en SharePoint 2013 worden niet gestart.

    - Als de werkstroom niet kan worden gestart, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers de werkstroom af en toe kunnen zien. Controleer het [Dashboard service status](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie van invloed is.

    - Als het probleem zich nog steeds voordoet, kunt u een ondersteuningsticket registreren als u meer dan 24 uur hebt verstreken sinds u het eerst hebt gezien. In veel gevallen werken we al met een oplossing. Geef ons minstens 24 uur om een oplossing te voltooien.

- SharePoint 2010-werkstromen vertraagd bij start.

    - Dit gebeurt als de werkstroom wordt geactiveerd in grote batches. (bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).

    - Werkstromen zijn niet ontworpen voor het uitvoeren van realtime en daarom is een vertraging inherent aan het ontwerp gedrag.

   -  Als de werkstroom complexe Extensible object Markup Language (XMOL) is, kan de compilatie traag worden. Raadpleeg [Dit](https://support.microsoft.com//kb/3043697) artikel.

    - U dient de werkstroom te vereenvoudigen of opnieuw te ontwerpen met het type Microsoft SharePoint 2013-werkstroom platform.

    - Als uw werkstroomgeschiedenis groot is geworden, kunt u de items verwijderen of een nieuwe geschiedenislijst maken.

        Meer informatie: [werkstroomgeschiedenis wissen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


