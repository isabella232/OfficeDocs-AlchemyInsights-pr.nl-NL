---
title: Problemen met het ontwikkelen van toepassingen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013419"
---
# <a name="issues-developing-applications"></a>Problemen met het ontwikkelen van toepassingen

Zie de volgende artikelen om de meest voorkomende problemen bij het Azure Active Directory (AD)-apps op te lossen:

- [Ik zie problemen bij het aanmelden bij toepassing(en) met alleen de Chrome-browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ik weet niet hoe ik de standaardinstellingen voor de levensduur van het token voor mijn toepassing moet wijzigen](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Ik ben in de war over de manier waarop toestemming voor toepassingen werkt](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ik weet niet hoe ik machtigingen voor mijn toepassing moet verlenen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ik begrijp het verschil tussen gedelegeerde en toepassingsmachtigingen niet](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)***

- Vanaf 30 juni 2020 worden er geen nieuwe functies meer toegevoegd aan Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph). We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

- Vanaf 30 juni 2022 wordt de ondersteuning voor ADAL en AAD Graph beëindigd en bieden we geen technische ondersteuning of beveiligingsupdates meer aan. Als gevolg van deze voorwaarde zijn de volgende gevolgen:

    - Apps met ADAL in bestaande versies van besturingssystemen blijven na deze tijd wel werken, maar krijgen geen technische ondersteuning of beveiligingsupdates.

    - Apps met AAD-Graph na deze tijd ontvangen mogelijk geen antwoorden meer van het AAD-Graph eindpunt

**ADAL-migratie**

Als u Microsoft-apps gebruikt, raden we u aan bij te werken naar de Microsoft Authentication Library (MSAL), met de nieuwste functies en beveiligingsupdates. Deze aanbeveling is in de context van Microsoft die het proces start om de apps te migreren naar MSAL tegen het einde van de ondersteuningsdeadline. 

De migratie door Microsoft van de apps naar MSAL zorgt ervoor dat de apps profiteren van de doorlopende beveiligings- en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL wordt gebruikt, raden we u aan de broncode van al uw apps te bekijken en, indien van toepassing, contact op te zoeken met onafhankelijke softwareleveranciers (ISV's) of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die AAD-Graph gebruiken, volgt u onze richtlijnen voor het migreren van AAD-Graph apps naar Microsoft Graph:

1. [De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncode van uw apps te bekijken en, indien van toepassing, contact op te zoeken met onafhankelijke softwareleveranciers (ISV's) of app-providers. Microsoft-ondersteuning kan u ook informatie geven over AAD Graph gebruik in uw tenant.







