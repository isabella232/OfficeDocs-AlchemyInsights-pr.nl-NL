---
title: Werkstroome-mail wordt niet verzonden
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
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766128"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Werkstroome-mail wordt niet verzonden voor een SharePoint-lijst of -bibliotheek

1. E-mail van werkstromen wordt niet naar alle gebruikers of alleen specifieke gebruikers verzonden of u ziet de fout **Het e-mailbericht kan niet worden verzonden. Controleer of de e-mail een geldige ontvanger heeft.**

    Controleer of de gebruiker bestaat in de groep Machtigingen **voor alle personen** (lijst met gebruikersgegevens) voor die siteverzameling.  Voorbeeld directe URL:<tenant><sitename>https:// .sharepoint.com/sites/ /_layouts/15/people.aspx? LidmaatschapGroupId=0

    - Als de gebruiker niet bestaat, controleert u of de gebruiker is aangemeld bij de pagina. 
    - Als het een externe gebruiker is, moet u ervoor zorgen dat de uitnodiging is geaccepteerd.
    - Als de gebruiker wel in de groep machtigingen aanwezig is, controleert u of het e-mailadres juist is.
    - Als het e-mailadres van de gebruikers hier niet is ingesteld, maakt u een voorbeeldwaarschuwing voor die gebruiker die de synchronisatie van dat gebruikersaccount van gebruikersprofielen van SharePoint naar deze siteverzameling dwingt.
 
2. E-mail van werkstromen wordt verzonden naar de beheerders van de siteverzameling, maar niet naar andere gebruikers en zie de fout **HTTP Verboden naar <span>https:</span>/URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Zie [Toegang geweigerd wanneer u een e-mail verzendt naar een SharePoint-groep](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Controleer ook of de **siteverzamelingsfunctie** voor beperkte toegang voor gebruikersmachtigingen niet actief is.


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft Flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


