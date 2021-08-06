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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907733"
---
# <a name="workflow-is-not-starting"></a>Werkstroom start niet

- SharePoint werkstromen voor 2010 en SharePoint 2013 worden niet begonnen.

    - Als uw werkstroom niet wordt begonnen, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers mogelijk met af en toe vertragingen met de voortgang van de werkstroom te maken kunnen krijgen. Controleer het [dashboard Service health om](https://admin.microsoft.com/AdminPortal/Home/servicehealth) te zien of uw organisatie wordt beïnvloed.

    - Als er meer dan 24 uur zijn verstreken sinds u dit probleem voor het eerst hebt gezien, moet u een ondersteuningsticket aanmelden. In veel gevallen werken we al aan een oplossing. Geef ons ten minste 24 uur om een oplossing te voltooien.

- SharePoint 2010-werkstromen vertraagd bij de start.

    - Dit gebeurt als de werkstroom wordt geactiveerd in grote batches. (bijvoorbeeld wanneer er meerdere items tegelijk worden toegevoegd).

    - Werkstromen zijn niet ontworpen om realtime uit te voeren, dus een vertraging is ontwerpgedrag.

   -  Als de werkstroom complex is Extensible Object Markup Language (XMOL), kan de compilatie traag zijn. Controleer [dit](https://support.microsoft.com//kb/3043697) artikel.

    - U moet de werkstroom vereenvoudigen of de werkstroom opnieuw ontwerpen met het type Werkstroomplatform van Microsoft SharePoint 2013.

    - Als de werkstroomgeschiedenis groot is geworden, kunt u de items verwijderen of een nieuwe geschiedenislijst maken.

        Meer informatie: [Werkstroomgeschiedenis verwijderen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Gerelateerde onderwerpen
Wilt u uw Microsoft Flow online SharePoint proberen?
- [Een Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
