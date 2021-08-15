---
title: Problemen met het ontwikkelen van toepassingen met API's
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013455"
---
# <a name="issues-developing-applications-with-apis"></a>Problemen met het ontwikkelen van toepassingen met API's

Als u wilt beginnen met Azure Active Directory Graph API, bekijkt u de [Handleiding snelstart](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) van Azure AD Graph API of bekijkt u de interactieve Documentatie van Azure [AD-Graph API-naslaginformatie.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)**

**Vanaf 30 juni 2020** worden er geen nieuwe functies meer toegevoegd aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

**Vanaf 30 juni 2022** beëindigen we de ondersteuning voor ADAL en Azure AD Graph en bieden we geen technische ondersteuning of beveiligingsupdates meer.

Apps met ADAL in bestaande versies van besturingssystemen blijven na deze tijd wel werken, maar krijgen geen technische ondersteuning of beveiligingsupdates.

Apps met Azure AD-Graph na deze tijd ontvangen mogelijk geen antwoorden meer van het Azure AD-Graph eindpunt.

**ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.

Als u Microsoft-apps gebruikt, weet dan dat Microsoft bezig is met het migreren van de toepassingen naar MSAL tegen het einde van de ondersteuningsdeadline, zodat ze profiteren van de voortdurende beveiligings- en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Meer informatie over het migreren van apps per platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL wordt gebruikt, raden we u aan de broncode van al uw apps te bekijken en indien van toepassing contact op te zoeken met isv's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die Azure AD-Graph gebruiken, volgt u onze richtlijnen voor het migreren van [Azure AD-Graph-apps](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)naar Microsoft Graph.

1. [De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle AAD-Graph in uw tenant.
1. Als uw app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of beheerder deze de juiste machtigingen verlenen via een toestemmingsproces. De [verwijzing Graph microsoft-machtigingen](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) bevat de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft-Graph API's. Het bevat ook richtlijnen voor het gebruik van de machtigingen.
