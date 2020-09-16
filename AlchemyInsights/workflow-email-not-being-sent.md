---
title: E-mail van werkstroom wordt niet verzonden
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
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748984"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail van werkstroom wordt niet verzonden voor een SharePoint-lijst of-bibliotheek

1. E-mail van werkstromen wordt niet naar alle gebruikers of alleen specifieke gebruikers verzonden of u ziet de fout **het e-mailbericht kan niet worden verzonden. Zorg ervoor dat het e-mailbericht een geldige geadresseerde heeft**.

    Controleer of de gebruiker in de groep machtigingen voor **alle personen** (gebruikersgegevens) voor die siteverzameling is opgenomen.  Voorbeeld van directe URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0

    - Als de gebruiker niet bestaat, moet u ervoor zorgen dat de gebruiker is aangemeld bij de pagina. 
    - Als het om een externe gebruiker gaat, controleert u of de uitnodiging is geaccepteerd.
    - Als de gebruiker in de groep machtigingen bestaat, controleert u of het e-mailadres juist is.
    - Als het e-mailadres van gebruikers hier niet is ingesteld, maakt u een voorbeeld waarschuwing voor de gebruiker, die de synchronisatie van die gebruikersaccount van gebruikersprofielen van SharePoint tot deze siteverzameling afdwingt.
 
2. E-mail van werkstromen wordt verzonden naar de beheerders van siteverzamelingen, maar niet naar andere gebruikers en zie de fout **http niet toegestaan voor <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Zie [toegang geweigerd wanneer u een e-mailbericht naar een SharePoint-groep verzendt](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Zorg er ook voor dat de functie voor het **vergrendelen van gebruikersmachtigingen voor gebruikers met beperkte toegang** niet is geactiveerd.


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u Microsoft flow uitproberen in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


