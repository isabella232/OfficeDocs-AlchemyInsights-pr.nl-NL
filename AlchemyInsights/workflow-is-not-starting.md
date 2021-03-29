---
title: Werkstroom start niet
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403738"
---
# <a name="workflow-is-not-starting"></a>Werkstroom start niet

- SharePoint 2010- en SharePoint 2013-werkstromen beginnen niet.

    - Als uw werkstroom niet wordt begonnen, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers mogelijk met af en toe vertragingen met de voortgang van de werkstroom te maken kunnen krijgen. Controleer het [dashboard Service health om](https://admin.microsoft.com/AdminPortal/Home/servicehealth) te zien of uw organisatie wordt beïnvloed.

    - Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst hebt gezien, moet u een ondersteuningsticket aanmelden. In veel gevallen werken we al aan een oplossing. Geef ons ten minste 24 uur om een oplossing te voltooien.

- SharePoint 2010-werkstromen zijn vertraagd bij de start.

    - Dit gebeurt als de werkstroom wordt geactiveerd in grote batches. (bijvoorbeeld wanneer er meerdere items tegelijk worden toegevoegd).

    - Werkstromen zijn niet ontworpen om realtime uit te voeren, dus een vertraging is ontwerpgedrag.

   -  Als de werkstroom complex is Extensible Object Markup Language (XMOL), kan de compilatie traag zijn. Controleer [dit](https://support.microsoft.com//kb/3043697) artikel.

    - U moet de werkstroom vereenvoudigen of deze opnieuw ontwerpen met behulp van het type Microsoft SharePoint 2013-werkstroomplatform.

    - Als de werkstroomgeschiedenis groot is geworden, kunt u de items verwijderen of een nieuwe geschiedenislijst maken.

        Meer informatie: [Werkstroomgeschiedenis verwijderen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft Flow proberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
