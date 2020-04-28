---
title: Dagelijkse e-maillimiet overschreden. De werkstroom wordt opgeschort.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908699"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-mail limiet overschreden. De werkstroom wordt opgeschort.

Deze fout kan worden ontvangen in de volgende scenario's:

- U hebt een werkstroom in SharePoint Online die het type SharePoint 2010- of SharePoint 2013-werkstroomplatform gebruikt.
- De werkstroom is geconfigureerd om een aangepast e-mailbericht te verzenden naar meer dan 200 gebruikers tegelijk, meer dan 10.000 ontvangers per dag of meer dan 30 berichten per minuut.
- Wanneer u de werkstroom uitvoert, wordt het e-mailbericht niet verzonden en ziet u het volgende gedrag:
    - Voor een werkstroom met het sharepoint-platformtype SharePoint 2013 bladert u naar de pagina **Werkstroomstatus.** Op de pagina Werkstroomstatus wordt de **interne status** ingesteld op **Gestart**en wordt de informatieballon niet naar een ontvanger **kunnen verzenden**.

Als u dit probleem wilt oplossen, configureert u uw werkstroom om e-mailberichten te verzenden zonder de [verzendlimieten van Exchange Online te](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)overschrijden. Gebruik bijvoorbeeld een pauze in de werkstroom, stuur de e-mail naar een Microsoft 365-groep, een distributiegroep of beveiligingsgroep met e-mail of stuur het bericht naar minder dan 200 ontvangers tegelijk.


Zie het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.

## <a name="related-topics"></a>Verwante onderwerpen
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 