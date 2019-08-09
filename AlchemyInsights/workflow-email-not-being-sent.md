---
title: Werkstroom e-mailbericht wordt niet verzonden
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
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270667"
---
# <a name="workflow-email-is-not-being-sent"></a>Werkstroom e-mailbericht wordt niet verzonden

1. E-mailadres van werkstromen worden niet verzonden naar alle gebruikers of alleen bepaalde gebruikers of ziet u dat de fout **het e-mailbericht kan niet worden verzonden. Controleer of het e-mailbericht heeft een geldige geadresseerde**.

    Controleer of de gebruiker in de machtigingsgroep **Alle mensen** (lijst met gebruikersgegevens) voor die siteverzameling bestaat.  Voorbeeld van een directe URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Als de gebruiker niet bestaat, moet u dat de gebruiker is aangemeld op de pagina. 
    - Zorg dat de uitnodiging is geaccepteerd als een externe gebruiker is.
    - Als de gebruiker in de machtigingsgroep bestaat, moet dat het e-mailadres juist is.
    - Als de gebruikers e-mailadres hier niet is ingesteld, maakt u een waarschuwing voor een monster voor die gebruiker, waardoor de synchronisatie van die account van gebruikers profielen van SharePoint voor deze siteverzameling.
 
2. E-mailadres van werkstromen worden verzonden naar beheerders van de siteverzameling, maar niet voor andere gebruikers en Zie de fout **verboden HTTP- <spam> <spam> ** <spam> <spam>.
 

    Zie [De toegang geweigerd wanneer verzonden e-mail naar groepen](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Controleer ook of de **modus met beperkte toegang gebruiker machtiging lockdown** siteverzamelingfunctie is niet actief.


## <a name="related-topics"></a>Verwante onderwerpen
Wilt u proberen Microsoft Flow in SharePoint Online?
- [Stroom maken](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint en stroom](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


