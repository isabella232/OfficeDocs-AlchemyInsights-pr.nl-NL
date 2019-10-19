---
title: De werkstroom wordt niet gestart
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738084"
---
# <a name="workflow-is-not-starting"></a>De werkstroom wordt niet gestart

- SharePoint 2010 en SharePoint 2013 werkstromen worden niet gestart.

    - Als uw werkstroom niet wordt gestart, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers periodieke vertragingen met workflowvoortgang kunnen ondervinden. Controleer de [service status dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie wordt beïnvloed.

    - Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst zag, logt u een ondersteuningsticket in. In veel gevallen werken we nu al aan een oplossing. Gelieve ons ten minste 24 uur te geven om een oplossing te voltooien.

- SharePoint 2010 werkstromen vertraagd bij het starten.

    - Dit gebeurt als de werkstroom wordt geactiveerd in grote batches. (bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).

    - Workflows zijn niet ontworpen om real-time uit te voeren, dus een vertraging is per ontwerp gedrag.

   -  Als de werkstroom complexe Extensible object Markup Language (XMOL) is, kan compilatie traag zijn. Raadpleeg [Dit](https://support.microsoft.com//kb/3043697) artikel.

    - U moet de werkstroom vereenvoudigen of opnieuw ontwerpen met het type werkstroom platform van Microsoft SharePoint 2013.

    - Als de werkstroomgeschiedenis groot is gegroeid, u de items verwijderen of een nieuwe geschiedenislijst maken.

        Meer informatie: [Workflowhistorie opschonen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


