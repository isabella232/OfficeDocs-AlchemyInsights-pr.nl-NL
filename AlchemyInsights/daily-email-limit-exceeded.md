---
title: Dagelijkse e-maillimiet overschreden. De werkstroom is opgeschort.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580328"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-maillimiet overschreden. De werkstroom is opgeschort.

Deze fout kan worden ontvangen in de volgende scenario's:

- U hebt een werkstroom in SharePoint Online die het type SharePoint 2010- of SharePoint 2013-werkstroom gebruikt.
- De werkstroom is geconfigureerd om een aangepast e-mailbericht te verzenden naar meer dan 200 gebruikers tegelijk, meer dan 10.000 ontvangers per dag of meer dan 30 berichten per minuut.
- Wanneer u de werkstroom uitvoert, wordt het e-mailbericht niet verzonden en ziet u het volgende gedrag:
    - Voor een werkstroom met het SharePoint 2013-platformtype bladert u naar de pagina **Werkstroomstatus.** Op de pagina Werkstroomstatus is de **interne status** ingesteld **op Gestart**en wordt met de informatieballon niet naar een ontvanger kunnen **worden verzonden.**

Als u dit probleem wilt oplossen, configureert u uw werkstroom om e-mailberichten te verzenden zonder de limieten voor [Exchange Online-afzenders](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)te overschrijden. Gebruik bijvoorbeeld een pauze in de werkstroom, stuur de e-mail naar een Microsoft 365-groep, een beveiligingsgroep met distributiegroep of e-mail ingeschakelde beveiligingsgroep of stuur het bericht naar minder dan 200 geadresseerden tegelijk.


Zie het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.

## <a name="related-topics"></a>Verwante onderwerpen
- [Flow maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 