---
title: Werkstroom wordt niet gestart
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766092"
---
# <a name="workflow-is-not-starting"></a>Werkstroom wordt niet gestart

- SharePoint 2010- en SharePoint 2013-werkstromen worden niet gestart.

    - Als uw werkstroom niet wordt gestart, kan er een tijdelijke serviceprobleem zijn waarbij gebruikers met tussenpozen vertragingen kunnen ondervinden bij de voortgang van de werkstroom. Controleer het [dashboard servicestatus](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of de impact van uw organisatie is.

    - Als er meer dan 24 uur zijn verstreken sinds je dit probleem voor het eerst zag, log dan een ondersteuningsticket in. In veel gevallen werken we al aan een oplossing. Geef ons minstens 24 uur om een oplossing te voltooien.

- SharePoint 2010-werkstromen vertraagd bij het starten.

    - Dit gebeurt als de werkstroom in grote batches wordt geactiveerd. (bijvoorbeeld wanneer meerdere items tegelijk worden toegevoegd).

    - Werkstromen zijn niet ontworpen om real-time uit te voeren, dus een vertraging is het ontwerpgedrag.

   -  Als de werkstroom complexe Extensible Object Markup Language (XMOL) is, kan de compilatie traag zijn. Check [dit](https://support.microsoft.com//kb/3043697) artikel.

    - U moet de werkstroom vereenvoudigen of opnieuw ontwerpen met het type Microsoft SharePoint 2013-werkstroomplatform.

    - Als uw werkstroomgeschiedenis groot is geworden, u de items verwijderen of een nieuwe geschiedenislijst maken.

        Meer informatie : [Werkstroomgeschiedenis wissen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft Flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


