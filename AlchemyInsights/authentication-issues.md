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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974311"
---
# <a name="authentication-issues"></a>Verificatieproblemen

**Zoeken naar informatie over de AADSTS-foutcodes die worden geretourneerd via de Azure Active Directory (Azure AD) beveiligingstokenservice (STS)?** Zie Logboeken van [Azure AD-verificatie en Autorisatiefout codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) voor informatie over AADSTS fout beschrijvingen, fixes en enkele voorgestelde tijdelijke oplossingen.

Autorisatiefouten kunnen verschillende oorzaken hebben, waarvan de meeste problemen met een 401-of 403-fout veroorzaken. De volgende problemen kunnen bijvoorbeeld leiden tot autorisatiefouten:

- Onjuiste [verwervings stromen voor toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Slecht geconfigureerde [machtigings zoekbereiken](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Onvoldoende [toestemming](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Voor het oplossen van veelvoorkomende autorisatiefouten voert u de stappen uit die het meest overeenkomen met de fout die u ontvangt. Meerdere stappen kunnen van toepassing zijn op een fout die u ontvangt.

- **ongeautoriseerde fout in 401: is uw token geldig?**

Zorg ervoor dat de app een geldig toegangstoken voor Microsoft Graph als onderdeel van de aanvraag presenteert. Deze fout betekent meestal dat het toegangstoken ontbreekt in de header van de HTTP-authenticatieaanvraag of dat de token ongeldig is of is verlopen. We raden u ten zeerste aan om de Microsoft Authentication Library (MSAL) te gebruiken voor het verkrijgen van een toegangstoken. Deze fout kan ook optreden als u een gedelegeerd toegangstoken probeert te gebruiken dat is toegewezen aan een persoonlijk Microsoft-account om toegang te krijgen tot een API die alleen ondersteuning biedt voor werk-of school accounts (organisatie accounts).

**403 niet toegestaan fout: hebt u de juiste set machtigingen gekozen?**

Zorg ervoor dat u de juiste set machtigingen hebt aangevraagd op basis van de API-oproepen van Microsoft Graph. De aanbevolen rechten voor het werken met machtigingen worden in alle onderwerpen met naslag methoden voor Microsoft Graph API geboden. Daarnaast moet de machtigingen van een gebruiker of beheerder aan de toepassing worden verleend. Machtigingen verlenen normaalgesproken plaats via een toestemming pagina of gebruik van de bladerende Azure Portal Application-registratie. Klik vanuit de Blade **instellingen** voor de toepassing op **vereiste machtigingen** en klik op **machtigingen verlenen**. Zie voor meer informatie:

- [Machtigingen voor Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Meer informatie over Azure AD-machtigingen en toestemming](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 niet-toegestane fout: er is een token aangeschaft voor de aangewezen machtigingen in de app?**

Zorg ervoor dat de typen machtigingen zijn aangevraagd of toegewezen aan het type toegangstoken dat door uw app is opgehaald. U wordt mogelijk gevraagd om app-machtigingen te gebruiken, maar met gedelegeerde interactieve code-tokens in plaats van client Credential flow tokens, of het aanvragen en verlenen van gedelegeerde machtigingen maar het gebruik van client Credential flow-tokens in plaats van gedelegeerde code transport tokens.

Zie voor meer informatie over het verkrijgen van tokens:

- [Toegang verkrijgen namens gebruikers en gedelegeerde machtigingen](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0-autorisatiecode stroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Toegang krijgen zonder een gebruiker (Demon service) en Toepassingsmachtigingen](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 niet toegestaan fout: wachtwoord opnieuw instellen**

Op dit moment zijn er geen bevoegdheden van een toepassing voor de service-to-service bevoegdheden waarmee gebruikerswachtwoorden opnieuw kunnen worden ingesteld. Deze Api's worden alleen ondersteund door de interactieve gedelegeerde code stromen met een aangemelde beheerder. Zie [machtigingen voor Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)voor meer informatie.

**403 niet toegestaan: heeft de gebruiker toegang en zijn ze een licentie?**

Voor gedelegeerde code stromen wordt door Microsoft Graph geëvalueerd of de aanvraag is toegestaan op basis van de machtigingen die aan de app zijn verleend en welke machtigingen de aangemelde gebruiker heeft. In het algemeen wordt met deze fout aangegeven dat de gebruiker niet voldoende bevoegd is voor het uitvoeren van de aanvraag **of** de gebruiker geen licentie heeft voor de gegevens die worden geopend. Alleen gebruikers met de vereiste machtigingen of licenties kunnen de aanvraag succesvol indienen.

**403 niet toegestaan: de juiste resource-API is geselecteerd.**

API-services zoals Microsoft Graph Controleer of de *AUD* claim (doelgroep) in het ontvangen toegangstoken overeenkomt met de waarde die voor zichzelf verwacht, en zo niet of een 403-fout. Er is een veelvoorkomende fout opgetreden bij het gebruik van een token dat is verkregen voor Azure AD Graph-Api's, Outlook Api's of SharePoint/OneDrive-Api's voor het bellen van Microsoft Graph (of omgekeerd). Zorg ervoor dat de bronnen (of het bereik) van de app een token verkrijgen voor overeenkomsten met de API die de app aanroept.

**400 ongeldige aanvraag of 403 niet toegestaan: heeft de gebruiker naleven van de beleidsregels voor voorwaardelijke toegang van de organisatie?**

Een gebruiker die op basis van het beleid voor voorwaardelijke toegang (CA) van een organisatie toegang heeft tot gegevens van Microsoft Graph via de app wordt mogelijk aangeraden voor aanvullende informatie die niet aanwezig is in het toegangstoken dat de app oorspronkelijk heeft aangeschaft. In dit geval ontvangt uw app een **400 met een *interaction_required*** fout tijdens het verkrijgen van een toegangstoken of een **403 met *Insufficient_claims*** fout bij het bellen met Microsoft Graph. In beide gevallen bevat de fout respons aanvullende informatie die kan worden weergegeven aan het geautoriseerde eindpunt om de gebruiker te laten weten of u aanvullende informatie nodig hebt (bijvoorbeeld verificatie via meerdere factoren of apparaatregistratie).

Zie voor meer informatie over voorwaardelijke toegang:

- [Voorwaarden voor voorwaardelijke toegang verwerken met MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Richtlijnen voor ontwikkelaars voor Azure Active Directory voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (Aad-grafiek)_* _

- Vanaf 30 juni 2020 worden niet langer nieuwe functies toegevoegd aan Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD-grafiek). We bieden technische ondersteuning en beveiligingsupdates, maar bieden geen functie-updates meer.
- Vanaf 30 juni 2022 wordt de ondersteuning voor ADAL en AAD-grafiek beëindigd en ontvangt u niet langer technische ondersteuning en beveiligingsupdates.
    - Apps die gebruikmaken van ADAL op bestaande versie van het besturingssysteem werken na dit moment nog niet, maar krijgen geen technische ondersteuning of beveiligingsupdates.
    - Apps die gebruikmaken van AAD-grafieken na dit tijdstip, kunnen mogelijk niet langer antwoorden ontvangen van het AAD-grafiek eindpunt.

_ *ADAL-migratie**

We raden u aan een update uit te voeren voor de [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), met de meest recente functies en beveiligingsupdates. Deze aanbevelingen bevindt zich in de context van Microsoft die de toepassingen migreert naar MSAL door de einde datum van de ondersteunings deadline. Het doel van de migratie van Microsoft apps naar MSAL is om ervoor te zorgen dat de apps profiteren van de voortdurende beveiliging en functieverbeteringen van MSAL.

- [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Meer informatie over hoe u apps migreert op een platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Als u meer informatie wilt over het gebruik van ADAL, raden we u aan alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers (Isv's) of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw Tenant bieden.

**Migratie van AAD-grafieken**

Voor toepassingen die gebruikmaken van AAD Graph, volgt u onze richtlijnen voor het [migreren van Azure AD Graph-apps naar Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Onze migratie controlelijst biedt een aantekening aan de slag](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- De registratie portal van Azure app toont welke toepassingen gebruikmaken van een AAD-grafiek. We raden u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met Isv's of app-providers. Microsoft-ondersteuning kan u ook de informatie over alle AAD-grafiek gebruik in uw Tenant bieden.

 










