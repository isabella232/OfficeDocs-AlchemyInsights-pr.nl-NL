---
title: Problemen met verificatiebibliotheken
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027999"
---
# <a name="issues-with-authentication-libraries"></a>Problemen met verificatiebibliotheken

1. [Microsoft identity platform verificatiebibliotheken](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) bevat door Microsoft ondersteunde en compatibele client- en middlewarebibliotheken.
2. De Microsoft Authentication Library (MSAL) ondersteunt verschillende [verificatiestromen](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) voor gebruik in verschillende toepassingsscenario's.
3. Als u tokens wilt verifiëren en verkrijgen, initialiseert u een nieuwe openbare of vertrouwelijke clienttoepassing in uw code. U kunt verschillende configuratieopties instellen wanneer u de client-app initialiseert in de Microsoft Authentication Library (MSAL). Zie Configuratieopties voor [toepassingen voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)**

**Vanaf 30 juni 2020** worden er geen nieuwe functies meer toegevoegd aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

**Vanaf 30 juni 2022** beëindigen we de ondersteuning voor ADAL en Azure AD Graph en bieden we geen technische ondersteuning of beveiligingsupdates meer.

Apps die ADAL gebruiken voor bestaande besturingssysteemversies blijven na deze tijd werken, maar krijgen geen *technische ondersteuning of beveiligingsupdates.*

Apps met Azure AD-Graph na deze tijd ontvangen mogelijk geen antwoorden meer van het Azure AD-Graph eindpunt.

**ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.

Als u Microsoft-apps gebruikt, weet dan dat Microsoft bezig is met het migreren van de toepassingen naar MSAL tegen het einde van de ondersteuningsdeadline, zodat ze profiteren van de voortdurende beveiligings- en functieverbeteringen van MSAL.

Zie voor meer informatie:

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL wordt gebruikt, raden we u aan de broncode van al uw apps te bekijken en indien van toepassing contact op te zoeken met isv's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die Azure AD-Graph gebruiken, volgt u onze richtlijnen voor het migreren van [Azure AD-Graph-apps](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)naar Microsoft Graph.

1. [Onze migratiecontrolelijst biedt een beginpunt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle AAD-Graph in uw tenant.
3. Als uw app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of beheerder deze de juiste machtigingen verlenen via een toestemmingsproces. De [verwijzing Graph microsoft-machtigingen](https://docs.microsoft.com/graph/permissions-reference) bevat de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft-Graph API's. Het bevat ook richtlijnen voor het gebruik van de machtigingen.
