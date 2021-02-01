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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063604"
---
# <a name="issues-with-authentication-libraries"></a>Problemen met verificatiebibliotheken

1. [In verificatiebibliotheken van Microsoft-identiteitsplatforms](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) worden door Microsoft ondersteunde en compatibele client- en middlewarebibliotheken vermeld.
2. De Microsoft Authentication Library (MSAL) ondersteunt verschillende [verificatiestromen](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) voor gebruik in verschillende toepassingsscenario's.
3. Als u tokens wilt verifiëren en verkrijgen, initialiseert u een nieuwe openbare of vertrouwelijke clienttoepassing in uw code. U kunt verschillende configuratieopties instellen wanneer u de client-app initialiseert in de Microsoft Authentication Library (MSAL). Zie de configuratieopties [voor toepassingen voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)**

**Vanaf 30 juni 2020** voegen we geen nieuwe functies meer toe aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigen en bieden we geen technische ondersteuning of beveiligingsupdates meer.

Apps met ADAL in bestaande besturingssysteemversies blijven werken na deze periode, maar krijgen geen technische *ondersteuning of beveiligingsupdates.*

Apps die na deze tijd Azure AD Graph gebruiken, ontvangen mogelijk geen reacties meer van het Azure AD Graph-eindpunt.

**ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.

Als u Microsoft-apps gebruikt, weet u dat Microsoft voor het einde van de ondersteuningsdeadline haar toepassingen naar MSAL migreert, zodat ze kunnen profiteren van de lopende beveiligings- en functieverbeteringen van MSAL.

Zie voor meer informatie:

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Als u hulp nodig hebt bij het gebruik van ADAL in uw apps, raden we u aan alle broncode van uw apps te controleren en, indien van toepassing, contact op te met alle ISV's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die gebruikmaken van Azure AD Graph volgt u onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [De controlelijst voor migratie biedt een beginpunt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst geven met alle AAD Graph-gebruik in uw tenant.
3. De app heeft alleen toegang tot gegevens in Microsoft Graph als de gebruiker of beheerder de juiste machtigingen verleent via een toestemmingsproces. De [naslag voor Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference) bevat de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft Graph-API's. Daarnaast vindt u hier richtlijnen voor het gebruik van de machtigingen.
