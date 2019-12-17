---
title: Dagelijkse e-mail limiet overschreden. Werkstroom is onderbroken.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053112"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-mail limiet overschreden. Werkstroom is onderbroken.

Deze fout kan worden ontvangen in de volgende scenario's:

- U hebt een werkstroom in SharePoint Online die gebruikmaakt van het type SharePoint 2010 of SharePoint 2013 werkstroom platform.
- De werkstroom is geconfigureerd voor het verzenden van een aangepast e-mail bericht naar meer dan 200 gebruikers tegelijk, meer dan 10.000 geadresseerden per dag of meer dan 30 berichten per minuut.
- Wanneer u de werkstroom uitvoert, wordt het e-mail bericht niet verzonden en ziet u het volgende gedrag:
    - Voor een werkstroom met behulp van het platformtype SharePoint 2013, bladert u naar de pagina **Workflowstatus** . Op de pagina Workflowstatus wordt de **interne status** ingesteld op **gestart**en wordt de informatieballon **niet verzonden naar een geadresseerde**.

U dit probleem omzeilen, configureert u uw werkstroom voor het verzenden van e-mail berichten zonder overschrijding van de [limieten voor Exchange Online-afzender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Gebruik bijvoorbeeld een pauze in de werkstroom, stuur het e-mail bericht naar een groep van Office 365, een distributiegroep of een beveiligingsgroep met e-mailadres, of verzend de berichten naar minder dan 200 geadresseerden tegelijk.


Zie het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.

## <a name="related-topics"></a>Verwante onderwerpen
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 