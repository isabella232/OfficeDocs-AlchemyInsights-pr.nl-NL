---
title: Dagelijkse e-mail limiet overschreden. Workflow is geschorst.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059634"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-mail limiet overschreden. Workflow is geschorst.

Deze fout kan worden ontvangen in de volgende scenario's:

- U hebt een werkstroom in SharePoint Online die de SharePoint 2010 of SharePoint 2013 workflow platform wordt gebruikt.
- De werkstroom is geconfigureerd voor een aangepast e-mailbericht verzenden naar meer dan 200 gebruikers op een moment, meer dan 10.000 geadresseerden per dag of meer dan 30 berichten per minuut.
- Tijdens het uitvoeren van de werkstroom het e-mailbericht niet verzonden en u ziet het volgende gedrag:
    - U bladert naar de pagina **Werkstroomstatus** voor een werkstroom met behulp van het type SharePoint 2013-platform. De **Interne Status** is ingesteld op **gestart**en de ballon van de informatie **kan niet worden verzonden naar een geadresseerde**wordt weergegeven op de pagina Werkstroomstatus.

U kunt dit probleem omzeilen, kunt u uw workflow voor het verzenden van e-mailberichten zonder overschrijding van de [grenzen van Exchange Online afzender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)configureren. Bijvoorbeeld een pauze in de workflow gebruikt het e-mailbericht verzenden naar een Office 365-groep, een distributiegroep of beveiligingsgroep e-mail is ingeschakeld of het bericht naar minder dan 200 geadresseerden per keer verzenden.


Raadpleeg het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.

## <a name="related-topics"></a>Verwante onderwerpen
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en stroom](https://flow.microsoft.com/blog/sharepoint-and-flow/) 