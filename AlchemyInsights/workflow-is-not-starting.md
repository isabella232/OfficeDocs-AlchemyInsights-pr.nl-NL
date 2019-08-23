---
title: Workflow wordt niet gestart.
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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557965"
---
# <a name="workflow-is-not-starting"></a>Workflow wordt niet gestart.

- SharePoint 2010 en SharePoint 2013 werkstromen zijn niet gestart.

    - Als de werkstroom niet wordt gestart, kan er een tijdelijke service probleem waar gebruikers periodieke vertragingen met de voortgang van de workflow ondervinden. Controleer of de [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien als uw organisatie wordt beïnvloed.

    - Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst zag, meld u een support ticket. In veel gevallen hebben werkt we aan een oplossing. Geef ons ten minste 24 uur om een oplossing te voltooien.

- Werkstromen in SharePoint 2010 vertraagd op start.

    - Dit gebeurt als de werkstroom wordt geactiveerd in grote hoeveelheden. (bijvoorbeeld wanneer meerdere items worden toegevoegd in een keer).

    - Werkstromen zijn niet ontworpen real-time, zodat een vertraging inherent aan het ontwerp gedrag is.

   -  Als de werkstroom wordt complexe Extensible Object Markup Language (XMOL), compilatie traag worden. Controleer [Dit](https://support.microsoft.com/en-us/kb/3043697) artikel.

    - U moet de werkstroom te vereenvoudigen of ontwerpen met behulp van het type Microsoft SharePoint 2013 Workflow platform.

    - Als de workflowgeschiedenis grote is gegroeid, kunt u de items permanent verwijderen of een nieuw geschiedenisoverzicht maken.

        Meer informatie: [workflowgeschiedenis leegmaken](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u proberen Microsoft Flow in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en stroom](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


