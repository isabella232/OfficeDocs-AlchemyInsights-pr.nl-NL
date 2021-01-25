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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974305"
---
# <a name="issues-developing-applications"></a>Problemen met het ontwikkelen van toepassingen

Zie de volgende artikelen voor informatie over het oplossen van veelvoorkomende problemen bij het maken van Azure Active Directory (AD)-apps:

- [Ik zie problemen met aanmelden bij toepassing (en) met alleen de Chrome-browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ik weet niet hoe ik de standaardwaarden van de token levensduur voor mijn toepassing Wijzig](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Ik weet niet hoe de instemming van de toepassing werkt](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ik weet niet hoe ik machtigingen voor de toepassing moet verlenen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ik weet het verschil tussen gedelegeerde en Toepassingsmachtigingen niet](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (Aad-grafiek)** _

- Vanaf 30 juni 2020 worden niet langer nieuwe functies toegevoegd aan Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD-grafiek). We bieden technische ondersteuning en beveiligingsupdates, maar bieden geen functie-updates meer.

- Vanaf 30 juni 2022 wordt de ondersteuning voor ADAL en AAD-grafiek beëindigd en ontvangt u niet langer technische ondersteuning en beveiligingsupdates. Als gevolg van deze voorwaarde zijn de consequenties het volgende:

    - Apps die gebruikmaken van ADAL op bestaande versie van het besturingssysteem werken na dit moment nog niet, maar krijgen geen technische ondersteuning of beveiligingsupdates.

    - Apps die gebruikmaken van AAD-grafiek na deze periode, kunnen mogelijk niet langer antwoorden ontvangen van het eindpunt van een AAD-grafiek

_ *ADAL-migratie**

Als u Microsoft apps gebruikt, raden we u aan een update uit te voeren voor de Microsoft Authentication Library (MSAL), met de meest recente functies en beveiligingsupdates. Deze aanbevelingen bevindt zich in de context van Microsoft die het proces voor het migreren van de apps naar MSAL door de einde datum van de ondersteuning te bieden. 

De migratie door Microsoft van zijn apps naar MSAL garandeert dat de apps gebruikmaken van de voortdurende beveiliging en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Meer informatie over hoe u apps migreert op een platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Als u hulp nodig hebt bij het begrijpen van de apps van ADAL, raden we u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers (Isv's) of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw Tenant bieden.

**Migratie van AAD-grafieken**

Voor toepassingen die gebruikmaken van AAD Graph, volgt u onze richtlijnen voor het migreren van AAD-grafiek-apps naar Microsoft Graph:

1. [Onze migratie controlelijst biedt een aantekening aan de slag](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. De registratie portal van Azure app toont welke toepassingen gebruikmaken van een AAD-grafiek. We raden u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers (Isv's) of app-providers. Microsoft-ondersteuning kan u ook informatie geven over het gebruik van AAD-grafieken in uw Tenant.







