---
title: De limiet voor dagelijkse e-mail is overschreden. Werkstroom wordt opgeschort.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914646"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagelijkse e-maillimiet overschreden. Werkstroom wordt opgeschort.

Deze fout kan in de volgende scenario's worden ontvangen:

- U hebt een werkstroom in SharePoint Online die het type SharePoint 2010 of SharePoint 2013-werkstroomplatform gebruikt.
- De werkstroom is geconfigureerd om een aangepast e-mailbericht te verzenden naar meer dan 200 gebruikers tegelijk, meer dan 10.000 geadresseerden per dag of meer dan 30 berichten per minuut.
- Wanneer u de werkstroom uitwerkt, wordt het e-mailbericht niet verzonden en ziet u het volgende gedrag:
    - Voor een werkstroom met het SharePoint platformtype 2013  bladert u naar de pagina Werkstroomstatus. Op de pagina Werkstroomstatus is de interne **status** ingesteld op **Gestart** en wordt de informatieballon Weergegeven Kan **niet naar een geadresseerde worden gestuurd.**

Als u dit probleem wilt oplossen, configureert u uw werkstroom om e-mailberichten te verzenden zonder de limieten [Exchange Online afzender te overschrijden.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Gebruik bijvoorbeeld een pauze in de werkstroom, verzend de e-mail naar een Microsoft 365-groep, een distributiegroep of beveiligingsgroep met e-mail, of verzend het bericht naar minder dan 200 geadresseerden tegelijk.


Zie het volgende artikel voor [meer informatie.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Gerelateerde onderwerpen
- [Een Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 