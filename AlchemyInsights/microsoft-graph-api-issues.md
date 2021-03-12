---
title: Problemen met Microsoft Graph API
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713700"
---
# <a name="microsoft-graph-api-issues"></a>Problemen met Microsoft Graph API

Dit onderwerp is mogelijk ook van toepassing op ontwikkelaars die nog steeds Azure AD Graph API gebruiken. Het wordt echter **ten zeerste** aanbevolen Microsoft Graph te gebruiken voor al uw adreslijst-, identiteits- en toegangsbeheerscenario's.

**Verificatie- of autorisatieproblemen**

- Als uw  app geen tokens kan verkrijgen om Microsoft Graph te bellen, kiest u Probleem met het verkrijgen van een Categorie voor toegangstoken **(Verificatie)** Microsoft Graph voor specifiekere hulp en ondersteuning voor dit onderwerp.
- Als uw app **401-** of 403-autorisatiefouten ontvangt bij het bellen van Microsoft Graph, kiest u de categorie Microsoft Graph API (Getting an access denied **error) voor** specifieke hulp en ondersteuning voor dit onderwerp.

**Ik wil Microsoft Graph gebruiken, maar ik weet niet zeker waar ik moet beginnen**

- [Overzicht van Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Overzicht van identiteits- en toegangsbeheer in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Aan de slag met het maken van Microsoft Graph-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Microsoft Graph-API's testen in uw tenant of een demo-tenant

**Ik wil Microsoft Graph gebruiken, maar ondersteunt het de v1.0-adreslijst-API's die ik nodig heb?**

Microsoft Graph is de aanbevolen API voor adreslijst-, identiteits- en toegangsbeheer. Er zijn echter nog steeds een paar hiaten tussen wat mogelijk is in Azure AD Graph en Microsoft Graph. Bekijk de volgende artikelen, waarin de meest recente verschillen worden belicht die u moet helpen bij uw keuze:

- [Verschillen in resourcetype tussen Azure AD Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Verschillen in eigenschap tussen Azure AD Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodeverschillen tussen Azure AD en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**De API die ik bel werkt niet. Waar kan ik meer tests uitvoeren?**

**Microsoft Graph Explorer-** Test Microsoft Graph API's in uw tenant of een demoten tenant en bekijk ook de voorbeeldquery's **in** Microsoft Graph Explorer.

**Mijn app is te traag en wordt vertraagd. Welke verbeteringen kan ik aanbrengen?**

Afhankelijk van uw scenario kunt u diverse opties kiezen om uw toepassing efficiënter te maken en om in sommige gevallen minder snel te worden beperkt door de service (wanneer u te veel oproepen doet).

- [Best practices voor Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchingaanvragen](https://docs.microsoft.com/graph/json-batching)
- [Wijzigingen bijhouden via deltaquery](https://docs.microsoft.com/graph/delta-query-overview)
- [Via webhoekken op de hoogte worden gesteld van wijzigingen](https://docs.microsoft.com/graph/webhooks)
- [Richtlijnen voor beperken](https://docs.microsoft.com/graph/throttling)

**Waar vind ik meer informatie over fouten en bekende problemen?**

- [Informatie over Microsoft Graph-foutreactie](https://docs.microsoft.com/graph/errors)
- [Bekende problemen met Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Waar kan ik de status van de beschikbaarheid en connectiviteit van de service controleren?**

De beschikbaarheid en connectiviteit van de onderliggende services die kunnen worden gebruikt via Microsoft Graph, kan van invloed zijn op de algehele beschikbaarheid en prestaties van Microsoft Graph.

- Controleer voor de servicestatus van Azure Active Directory de status van de beveiligings- en **identiteitsservices** die worden weergegeven op de [statuspagina van Azure.](https://azure.microsoft.com/status/)
- Voor Office-services die bijdragen aan Microsoft Graph controleert u de status van de services die worden weergegeven in het [Dashboard voor servicestatus van Office.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph-autorisatiefouten kunnen het gevolg zijn van verschillende problemen, waarvan de meeste een 401- of 403-fout genereren. Het volgende kan bijvoorbeeld leiden tot autorisatiefouten:

- Onjuiste [verwervingsstromen van toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Slecht geconfigureerde [machtigingsbereiken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Geen [toestemming](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)_* _

_*Vanaf 30 juni 2020** voegen we geen nieuwe functies meer toe aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.

**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigen en bieden we geen technische ondersteuning of beveiligingsupdates meer.

Apps met ADAL in bestaande besturingssysteemversies blijven werken na deze periode, maar krijgen geen technische *ondersteuning of beveiligingsupdates.*

Apps die na deze tijd Azure AD Graph gebruiken, ontvangen mogelijk geen reacties meer van het Azure AD Graph-eindpunt.

**ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.

Als u Microsoft-apps gebruikt, weet u dat Microsoft voor het einde van de ondersteuningsdeadline haar toepassingen naar MSAL migreert, zodat ze kunnen profiteren van de lopende beveiligings- en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Als u hulp nodig hebt bij het gebruik van ADAL in uw apps, raden we u aan alle broncode van uw apps te bekijken en, indien van toepassing, contact op te met alle ISV's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Voor toepassingen die Gebruikmaken van Azure AD Graph volgt u onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst geven met alle AAD Graph-gebruik in uw tenant.
3. De app heeft alleen toegang tot gegevens in Microsoft Graph als de gebruiker of beheerder de juiste machtigingen verleent via een toestemmingsproces. De [microsoft Graph-machtigingenverwijzing bevat](https://docs.microsoft.com/graph/permissions-reference) de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft Graph-API's. Daarnaast vindt u hier richtlijnen voor het gebruik van de machtigingen.
