---
title: Verificatieproblemen
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
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976844"
---
# <a name="authentication-issues"></a>Verificatieproblemen

**Zoekt u informatie over de AADSTS-foutcodes die worden geretourneerd van de Azure Active Directory (Azure AD) beveiligingstokenservice (security token service, STS)?** Zie [Azure AD-verificatie en -foutcodes voor autorisatie](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) om foutbeschrijvingen van AADSTS, oplossingen en enkele voorgestelde tijdelijke oplossingen te vinden.

Autorisatiefouten kunnen het gevolg zijn van verschillende problemen, waarvan de meeste een 401- of 403-fout genereren. De volgende problemen kunnen bijvoorbeeld leiden tot autorisatiefouten:

- Onjuiste [verwervingsstromen van toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Slecht geconfigureerde [machtigingsbereiken](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Geen [toestemming](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Als u veelvoorkomende autorisatiefouten wilt oplossen, volgt u de onderstaande stappen die het meest overeenkomen met de fout die u ontvangt. Er kunnen meerdere stappen van toepassing zijn op een fout die u ontvangt.

**401 Onbevoegdheidsfout: Is uw token geldig?**

Controleer of uw app een geldig toegangstoken voor Microsoft Graph presenteert als onderdeel van de aanvraag. Deze fout betekent vaak dat het toegangstoken ontbreekt in de koptekst voor de HTTP-verificatieaanvraag of dat het token ongeldig of verlopen is. Het wordt ten zeerste aangeraden de Microsoft Authentication Library (MSAL) te gebruiken voor het verkrijgen van toegangstokens. Daarnaast kan deze fout optreden als u probeert een gedelegeerd toegangstoken te gebruiken dat is verleend aan een persoonlijk Microsoft-account voor toegang tot een API die alleen ondersteuning biedt voor werk- of schoolaccounts (organisatieaccounts).

**403 Fout verboden: Hebt u de juiste set machtigingen gekozen?**

Controleer of u de juiste set machtigingen hebt aangevraagd op basis van de Microsoft Graph API's die u met de app aanroept. Aanbevolen machtigingen met de minste bevoegdheden worden gegeven in alle onderwerpen over naslagmethodes voor Microsoft Graph API. Daarnaast moeten deze machtigingen aan de toepassing worden verleend door een gebruiker of een beheerder. Het verlenen van machtigingen gebeurt gewoonlijk via een toestemmingspagina of het gebruik van de registratieprocedure van de Azure Portal-toepassing. Klik bij de **Instellingen** van de toepassing op **Vereiste machtigingen** en klik vervolgens op **Verkregen machtigingen**. Zie voor meer informatie:

- [Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD-machtigingen en -toestemming begrijpen](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Fout verboden: Heeft uw app een token verkregen die overeenkomt met de gekozen machtigingen?**

Zorg ervoor dat de typen machtigingen die zijn aangevraagd of verleend, overeenkomen met het type toegangstoken dat uw app krijgt. Het kan zijn dat u appmachtigingen aanvraagt en verleent, maar gedelegeerde tokens voor de interactieve codestroom in plaats van tokens voor de clientreferentiestroom gebruikt. Of u vraagt gedelegeerde machtigingen aan en verleent deze, maar gebruikt clientreferentiestroomtokens in plaats van gedelegeerde codestroomtokens.

Voor meer informatie over het verkrijgen van tokens, gaat u naar:

- [Toegang krijgen namens gebruikers en gedelegeerde machtigingen](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 autorisatiecodestroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Toegang krijgen zonder een gebruiker (daemon-service) en toepassingsmachtigingen](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0-clientreferentiestroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Fout verboden: Wachtwoord opnieuw instellen**

Momenteel zijn er geen daemon-service-to-servicemachtigingen voor toepassingen waarmee gebruikerswachtwoorden opnieuw kunnen worden ingesteld. Deze API's worden alleen ondersteund met behulp van interactieve, gedelegeerde codestromen met een aangemelde beheerder. Zie [Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference) voor meer informatie.

**403 Verboden: Heeft de gebruiker toegang en een licentie?**

Voor gedelegeerde codestromen evalueert Microsoft Graph of de aanvraag is toegestaan op basis van de machtigingen die aan de app zijn verleend en de machtigingen die de aangemelde gebruiker heeft. Over het algemeen geeft deze fout aan dat de gebruiker niet voldoende bevoegdheden heeft om de aanvraag uit te voeren **of** dat de gebruiker geen licentie heeft voor de gegevens die worden gebruikt. Alleen gebruikers met de vereiste machtigingen of licenties kunnen de aanvraag indienen.

**403 Verboden: Hebt u de juiste resource-API geselecteerd?**

API-services zoals Microsoft Graph controleren of de claim van de *doelgroep* in het ontvangen toegangstoken overeenkomt met de waarde die wordt verwacht, en als dit niet het geval is, treedt er een 403-fout Verboden op. Een veelvoorkomende fout die deze foutmelding tot gevolg heeft, is het gebruik van een token dat is verkregen voor Azure AD Graph-API's, Outlook-API's of SharePoint/OneDrive-API's om Microsoft Graph aan te roepen (of omgekeerd). Zorg ervoor dat de resource (of het bereik) waar de app een token voor verkrijgt, overeenkomt met de API die door de app wordt aangeroepen.

**400 Slechte aanvraag of 403 Verboden: Voldoet de gebruiker aan het beleid voor voorwaardelijke toegang (conditional access, CA) van de organisatie?**

Op basis van het beleid voor voorwaardelijke toegang (CA) van een organisatie, heeft een gebruiker die via uw app toegang heeft tot Microsoft Graph-bronnen mogelijk beperkte toegang tot aanvullende informatie die niet aanwezig is in het toegangstoken dat de app oorspronkelijk heeft verkregen. In dit geval ontvangt uw app een **400 met een *interaction_required***-fout tijdens het verkrijgen van toegangstokens of een **403 met *insufficient_claims***-fout bij het aanroepen van Microsoft Graph. In beide gevallen bevat het foutbericht aanvullende informatie die kan worden gepresenteerd aan het geautoriseerde eindpunt om de gebruiker om aanvullende informatie te vragen (zoals meervoudige verificatie of apparaatinschrijvingen).

Voor meer informatie over voorwaardelijke toegang, gaat u naar:

- [Problemen met voorwaardelijke toegang verwerken met MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Ontwikkelaarsbegeleiding voor voorwaardelijke toegang Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)_* _

- Vanaf 30 juni 2020 worden er geen nieuwe functies meer toegevoegd aan Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph). We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.
- Vanaf 30 juni 2022 wordt de ondersteuning voor ADAL en AAD Graph beëindigd en bieden we geen technische ondersteuning of beveiligingsupdates meer aan.
    - Apps met ADAL in bestaande versies van besturingssystemen blijven na deze tijd wel werken, maar krijgen geen technische ondersteuning of beveiligingsupdates.
    - Apps die na deze tijd gebruikmaken van AAD Graph ontvangen mogelijk geen reacties meer van het AAD Graph-eindpunt.

_ *ADAL-migratie**

U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat. Deze aanbeveling maakt deel uit van de context waarin Microsoft de toepassingen migreert naar MSAL voor het einde van de ondersteuningsdeadline. Het doel van de migratie van Microsoft-apps naar MSAL is ervoor te zorgen dat de apps profiteren van de continue beveiligings- en functieverbeteringen van MSAL.

- [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Meer informatie over het per platform migreren van apps](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Als u hulp nodig hebt bij het gebruik van ADAL in de apps, raden we u aan alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.

**AAD Graph-migratie**

Volg onze richtlijnen voor toepassingen die gebruikmaken van AAD Graph om [Azure AD Graph-apps te migreren naar Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph. Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers. Microsoft-ondersteuning kan u ook de informatie geven over het gebruik van AAD Graph in uw tenant.

 










