---
title: Dagelijkse e-mail limiet is overschreden. Werkstroom is opgeschort.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731558"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-mail limiet is overschreden. Werkstroom is opgeschort.

Deze fout kan worden weergegeven in de volgende scenario's:

- U hebt een werkstroom in SharePoint Online die het type SharePoint 2010 of SharePoint 2013-werkstroom platform gebruikt.
- De werkstroom is geconfigureerd voor het verzenden van een aangepast e-mailbericht naar meer dan 200 gebruikers tegelijk, meer dan 10.000 geadresseerden per dag, of meer dan 30 berichten per minuut.
- Wanneer u de werkstroom uitvoert, wordt het e-mailbericht niet verzonden en ziet u het volgende gedrag:
    - Voor een werkstroom met het platformtype SharePoint 2013, bladert u naar de pagina **werkstroom status** . Op de pagina werkstroom status wordt de **interne status** ingesteld op **gestart**en wordt de informatie ballon **niet naar een geadresseerde verzonden**.

Om dit probleem tijdelijk op te lossen, configureert u uw werkstroom voor het verzenden van e-mailberichten zonder dat de [afzenders van Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)worden overschreden Met een onderbreking in de werkstroom kunt u bijvoorbeeld de e-mail verzenden naar een Microsoft 365-groep, een distributiegroep of een beveiligingsgroep met e-mail, of het bericht verzenden naar minder dan 200 geadresseerden tegelijk.


Zie het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.

## <a name="related-topics"></a>Verwante onderwerpen
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 