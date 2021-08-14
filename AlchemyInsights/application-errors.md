---
title: Toepassingsfouten
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
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931444"
---
# <a name="application-errors"></a>Toepassingsfouten

Zoekt u informatie over de **AADSTS-foutcodes** die worden geretourneerd uit de Azure Active Directory (Azure AD) security token service (STS)? Lees [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.

Autorisatiefouten kunnen het gevolg zijn van verschillende problemen, waarvan de meeste een 401- of 403-fout genereren. Het volgende kan bijvoorbeeld leiden tot autorisatiefouten:

- Onjuiste [verwervingsstromen van toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Slecht geconfigureerde [machtigingsbereiken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Geen [toestemming](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Als u veelvoorkomende autorisatiefouten wilt oplossen, probeert u de onderstaande stappen die het meest overeenkomt met de fout die u ontvangt. Er kunnen meer dan één van toepassing zijn.

**401 Onbevoegdheidsfout: Is uw token geldig?**

Zorg ervoor dat uw toepassing een geldig toegangs token voor Microsoft-Graph als onderdeel van de aanvraag presenteert. Deze fout betekent vaak dat het toegangstoken ontbreekt in de koptekst voor de HTTP-verificatieaanvraag of dat het token ongeldig of verlopen is. We raden u ten zeerste aan om de [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) te gebruiken voor het verkrijgen van toegangs tokens. Daarnaast kan deze fout optreden als u probeert een gedelegeerd toegangs token te gebruiken dat is verleend aan een persoonlijk Microsoft-account om toegang te krijgen tot een API die alleen werk- of schoolaccounts (organisatieaccounts) ondersteunt.

**403 Fout verboden: Hebt u de juiste set machtigingen gekozen?**

Controleer of u de juiste set machtigingen hebt aangevraagd op basis van de Microsoft-Graph API's voor uw app-oproepen. Aanbevolen minst bevoorrechte machtigingen worden verstrekt in alle onderwerpen van de Microsoft-Graph API-verwijzingsmethode. Daarnaast moeten deze machtigingen aan de toepassing worden verleend door een gebruiker of een beheerder. Het verlenen van machtigingen gebeurt normaal gesproken via een toestemmingspagina of door machtigingen toe te staan met behulp van het registratieblad van de Azure Portal-toepassing. Klik bij de **Instellingen** van de toepassing op **Vereiste machtigingen** en klik vervolgens op **Verkregen machtigingen**.

- [Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD-machtigingen en -toestemming begrijpen](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Fout verboden: Heeft uw app een token verkregen die overeenkomt met de gekozen machtigingen?**

Zorg ervoor dat het type machtigingen dat is aangevraagd of verleend overeenkomt met het type toegangs token dat uw app verkrijgt. Mogelijk vraagt en verleent u toepassingsmachtigingen, maar gebruikt u gedelegeerde interactieve codestroomtokens in plaats van clientreferentiestroomtokens, of vraagt u gedelegeerde machtigingen aan, maar gebruikt u clientreferentiestroomtokens in plaats van gedelegeerde codestroomtokens.

- [Toegang krijgen namens gebruikers en gedelegeerde machtigingen](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 autorisatiecodestroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Toegang krijgen zonder een gebruiker (daemon-service) en toepassingsmachtigingen](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0-clientreferentiestroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Fout verboden: Wachtwoord opnieuw instellen**

Momenteel zijn er geen daemon-service-to-servicemachtigingen voor toepassingen waarmee gebruikerswachtwoorden opnieuw kunnen worden ingesteld. Deze API's worden alleen ondersteund met behulp van interactieve, gedelegeerde codestromen met een aangemelde beheerder.

- [Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference)

**403 Verboden: Heeft de gebruiker toegang en een licentie?**

Voor gedelegeerde codestromen wordt Graph of de aanvraag is toegestaan op basis van de machtigingen die aan de app zijn verleend en de machtigingen die de aangemelde gebruiker heeft. Over het algemeen geeft deze fout aan dat de gebruiker niet voldoende bevoegdheden heeft om de aanvraag uit te voeren of dat de gebruiker geen licentie heeft voor de gegevens die worden gebruikt. Alleen gebruikers met de vereiste machtigingen of licenties kunnen de aanvraag indienen.

**403 Verboden: Hebt u de juiste resource-API geselecteerd?**

API-services zoals Microsoft Graph controleren of de aud-claim (doelgroep) in het ontvangen toegangs token overeenkomt met de waarde die ze voor zichzelf verwacht, en zo niet, resulteert dit in een fout van 403 Verboden. Een veelvoorkomende fout die deze foutmelding tot gevolg heeft, is het gebruik van een token dat is verkregen voor Azure AD Graph-API's, Outlook-API's of SharePoint/OneDrive-API's om Microsoft Graph aan te roepen (of omgekeerd). Zorg ervoor dat de resource (of het bereik) waar de app een token voor verkrijgt, overeenkomt met de API die door de app wordt aangeroepen.

**400 Slechte aanvraag of 403 Verboden: Voldoet de gebruiker aan het beleid voor voorwaardelijke toegang (conditional access, CA) van de organisatie?**

Op basis van het CA-beleid van een organisatie kan een gebruiker die toegang heeft tot Microsoft Graph-bronnen via uw app worden aangevochten voor aanvullende informatie die niet aanwezig is in het access-token dat uw app oorspronkelijk heeft verkregen. In dit geval ontvangt uw app een 400 met een *interaction_required*-fout tijdens het verkrijgen van toegangstokens of een 403 met *insufficient_claims*-fout bij het aanroepen van Microsoft Graph. In beide gevallen bevat de foutreactie aanvullende informatie die kan worden gepresenteerd aan het geautoriseerde eindpunt om de gebruiker uit te dagen voor aanvullende informatie (zoals meervoudige verificatie of apparaatinschrijving).

- [Problemen met voorwaardelijke toegang afhandelen met MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Ontwikkelaarsbegeleiding voor voorwaardelijke toegang Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
