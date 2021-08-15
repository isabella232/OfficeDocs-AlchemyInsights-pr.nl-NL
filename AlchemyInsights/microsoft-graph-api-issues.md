---
title: Microsoft Graph API-problemen
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975888"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API-problemen

Dit onderwerp kan ook van toepassing zijn op ontwikkelaars die nog steeds Azure AD Graph API. U wordt echter **ten zeerste** aangeraden Microsoft-Graph te gebruiken voor al uw adreslijst-, identiteits- en toegangsbeheerscenario's.

**Problemen met verificatie of autorisatie**

- Als uw  app geen tokens kan verkrijgen om Microsoft Graph te bellen, kiest u Probleem met het verkrijgen van een access **token (Authentication)** Microsoft Graph-categorie voor meer specifieke hulp en ondersteuning voor dit onderwerp.
- Als uw app **401 of 403** autorisatiefouten ontvangt bij het bellen van Microsoft Graph, kiest u de categorie Toegang geweigerde fout **(Autorisatie)** microsoft Graph API voor meer specifieke hulp en ondersteuning voor dit onderwerp.

**Ik wil Microsoft-Graph gebruiken, maar weet niet waar ik moet beginnen**

- [Overzicht van Microsoft-Graph](https://docs.microsoft.com/graph/overview)
- [Overzicht van identiteits- en accessbeheer in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Aan de slag met het bouwen Graph Microsoft-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Microsoft-Graph testen in uw tenant of een demo-tenant

**Ik wil Microsoft-Graph gebruiken, maar ondersteunt het de v1.0 directory-API's die ik nodig heb?**

Microsoft Graph is de aanbevolen API voor adreslijst-, identiteits- en toegangsbeheer. Er zijn echter nog enkele verschillen tussen wat er mogelijk is in Azure AD Graph en Microsoft Graph. Bekijk de volgende artikelen, waarin de meest recente verschillen worden belicht om u te helpen bij uw keuze:

- [Verschillen in resourcetype tussen Azure AD-Graph en Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschappenverschillen tussen Azure AD-Graph en Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodeverschillen tussen Azure AD en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**De API die ik bel werkt niet, waar kan ik meer testen?**

**Microsoft Graph Explorer-** Test Microsoft Graph API's in uw tenant of een demoten tenant en bekijk ook de voorbeeldquery's **in** Microsoft Graph Explorer.

**Mijn app is te traag en wordt ook beperkt. Welke verbeteringen kan ik aanbrengen?**

Afhankelijk van uw scenario zijn er diverse opties beschikbaar om uw toepassing performanter te maken en in sommige gevallen minder geneigd om te worden beperkt door de service (wanneer u te veel gesprekken voert).

- [Microsoft Graph best practices](https://docs.microsoft.com/graph/best-practices-concept)
- [Batching requests](https://docs.microsoft.com/graph/json-batching)
- [Wijzigingen bijhouden via deltaquery](https://docs.microsoft.com/graph/delta-query-overview)
- [Ontvang een melding van wijzigingen via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Richtlijnen voor beperking](https://docs.microsoft.com/graph/throttling)

**Waar vind ik meer informatie over fouten en bekende problemen?**

- [Microsoft Graph foutreactiegegevens](https://docs.microsoft.com/graph/errors)
- [Bekende problemen met Microsoft-Graph](https://docs.microsoft.com/graph/known-issues)

**Waar kan ik de status van de beschikbaarheid en connectiviteit van de service controleren?**

De beschikbaarheid en connectiviteit van de onderliggende services die via Microsoft-Graph kunnen worden gebruikt, kunnen van invloed zijn op de algehele beschikbaarheid en prestaties van Microsoft Graph.

- Voor Azure Active Directory servicestatus controleert u de status van **beveiligings- en identiteitsservices** die worden vermeld op de [pagina Azure-status.](https://azure.microsoft.com/status/)
- Voor Office services die bijdragen aan Microsoft-Graph, controleert u de status van services die worden vermeld in [het Office Servicestatusdashboard.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph autorisatiefouten kunnen het gevolg zijn van verschillende problemen, waarvan de meeste een fout van 401 of 403 genereren. Het volgende kan bijvoorbeeld leiden tot autorisatiefouten:

- Onjuiste [verwervingsstromen van toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Slecht geconfigureerde [machtigingsbereiken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Geen [toestemming](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)***

**Vanaf 30 juni 2020** worden er geen nieuwe functies meer toegevoegd aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

**Vanaf 30 juni 2022** beëindigen we de ondersteuning voor ADAL en Azure AD Graph en bieden we geen technische ondersteuning of beveiligingsupdates meer.

Apps die ADAL gebruiken voor bestaande besturingssysteemversies blijven na deze tijd werken, maar krijgen geen *technische ondersteuning of beveiligingsupdates.*

Apps met Azure AD-Graph na deze tijd ontvangen mogelijk geen antwoorden meer van het Azure AD-Graph eindpunt.

**ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.

Als u Microsoft-apps gebruikt, weet dan dat Microsoft bezig is met het migreren van de toepassingen naar MSAL tegen het einde van de ondersteuningsdeadline, zodat ze profiteren van de voortdurende beveiligings- en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL wordt gebruikt, raden we u aan de broncode van al uw apps te bekijken en indien van toepassing contact op te zoeken met isv's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die Azure AD-Graph gebruiken, volgt u onze richtlijnen voor het migreren van [Azure AD-Graph-apps](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)naar Microsoft Graph.

1. [De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle AAD-Graph in uw tenant.
3. Als uw app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of beheerder deze de juiste machtigingen verlenen via een toestemmingsproces. De [verwijzing Graph microsoft-machtigingen](https://docs.microsoft.com/graph/permissions-reference) bevat de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft-Graph API's. Het bevat ook richtlijnen voor het gebruik van de machtigingen.
