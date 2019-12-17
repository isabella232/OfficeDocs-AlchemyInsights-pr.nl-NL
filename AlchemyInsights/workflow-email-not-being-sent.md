---
title: Werkstroom-e-mail wordt niet verzonden
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049368"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Werkstroom-e-mail wordt niet verzonden voor een SharePoint-lijst of-bibliotheek

1. E-mail van werkstromen wordt niet verzonden naar alle gebruikers of alleen specifieke gebruikers, of u ziet de fout **die het e-mail bericht kan niet worden verzonden. Zorg ervoor dat het e-mail bericht een geldige geadresseerde heeft**.

    Controleer of de gebruiker bestaat in de groep **alle personen** machtigingen (lijst met gebruikersgegevens) voor die siteverzameling.  Voorbeeld van directe URL<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/people.aspx? MembershipGroupId = 0

    - Als de gebruiker niet bestaat, controleert u of de gebruiker is aangemeld bij de pagina. 
    - Als het een externe gebruiker is, controleert u of de uitnodiging is geaccepteerd.
    - Als de gebruiker in de groep machtigingen bestaat, controleert u of het e-mailadres juist is.
    - Als het e-mailadres van gebruikers hier niet is ingesteld, maakt u een voorbeeld waarschuwing voor die gebruiker die de synchronisatie van dat gebruikersaccount van gebruikersprofielen van SharePoint naar deze siteverzameling dwingt.
 
2. E-mail van workflows worden verzonden naar de beheerders van de siteverzameling, maar niet naar andere gebruikers en zien de fout **http verboden <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Zie [toegang geweigerd wanneer u een e-mail bericht naar een SharePoint-groep verzendt](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Controleer ook of de site verzamelings functie voor **beperkte toegang tot de vergrendelingsmodus van gebruikers** niet actief is.


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


