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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984541"
---
# <a name="application-errors"></a>Toepassingsfouten

Zoeken naar informatie over de **AADSTS-foutcodes** die worden geretourneerd via de Azure Active Directory (Azure AD) beveiligingstokenservice (STS)? U kunt de [foutcodes van Azure AD Authentication en Authorization](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) lezen voor het vinden van fout beschrijvingen van AADSTS, fixes en enkele voorgestelde tijdelijke oplossingen.

Autorisatiefouten kunnen verschillende oorzaken hebben, waarvan de meeste problemen met een 401-of 403-fout veroorzaken. In het volgende voorbeeld kunnen autorisatiefouten worden vastgelegd:

- Onjuiste [verwervings stromen voor toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Slecht geconfigureerde [machtigings zoekbereiken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Onvoldoende [toestemming](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Voor het oplossen van veelvoorkomende autorisatiefouten voert u de stappen uit die het meest overeenkomen met de fout die u ontvangt. Meer dan één kan van toepassing zijn.

**ongeautoriseerde fout in 401: is uw token geldig?**

Zorg ervoor dat de toepassing een geldig toegangstoken voor Microsoft Graph als onderdeel van de aanvraag presenteert. Deze fout betekent meestal dat het toegangstoken ontbreekt in de header van de HTTP-authenticatieaanvraag of dat de token ongeldig is of is verlopen. We raden u ten zeerste aan om de [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) te gebruiken voor het verkrijgen van een toegangstoken. Ook deze fout kan optreden als u een gedelegeerd toegangstoken probeert te gebruiken dat is toegewezen aan een persoonlijk Microsoft-account om toegang te krijgen tot een API die alleen ondersteuning biedt voor werk-of school accounts (organisatie accounts).

**403 niet toegestaan fout: hebt u de juiste set machtigingen gekozen?**

Controleer of u de juiste set machtigingen hebt aangevraagd op basis van de API-oproepen van Microsoft Graph. Aanbevolen beperkte machtigingen voor machtigingen worden vermeld in alle onderwerpen over de Microsoft Graph API Reference method. Daarnaast moet de machtigingen van een gebruiker of beheerder aan de toepassing worden verleend. Machtigingen verlenen normaalgesproken plaats via een machtigings pagina of door het verlenen van machtigingen via de Blade van de Azure-Portal toepassing. Klik vanuit de Blade **instellingen** voor de toepassing op **vereiste machtigingen** en klik op **machtigingen verlenen**.

- [Machtigingen voor Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Meer informatie over Azure AD-machtigingen en toestemming](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 niet-toegestane fout: er is een token aangeschaft voor de aangewezen machtigingen in de app?**

Zorg ervoor dat de aangevraagde of gebezite machtigingen van het type toegangstoken overeenkomen met uw app. U moet mogelijk aanvragen voor de toepassing en het verlenen van toepassingen, maar het gebruik van tokens in de client Credential flow, en het aanvragen en verlenen van gemachtigde machtigingen, maar het gebruik van client Credential flow-tokens in plaats van gedelegeerde code transport tokens

- [Toegang verkrijgen namens gebruikers en gedelegeerde machtigingen](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0-autorisatiecode stroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Toegang krijgen zonder een gebruiker (Demon service) en Toepassingsmachtigingen](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 niet toegestaan fout: wachtwoord opnieuw instellen**

Op dit moment zijn er geen bevoegdheden van een toepassing voor de service-to-service bevoegdheden waarmee gebruikerswachtwoorden opnieuw kunnen worden ingesteld. Deze Api's worden alleen ondersteund door de interactieve gedelegeerde code stromen met een aangemelde beheerder.

- [Machtigingen voor Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 niet toegestaan: heeft de gebruiker toegang en zijn ze een licentie?**

Voor gedelegeerde code stromen wordt in Microsoft Graph geëvalueerd of de aanvraag is toegestaan op basis van de machtigingen die aan de app zijn verleend en de machtigingen die de aangemelde gebruiker heeft. In het algemeen wordt met deze fout aangegeven dat de gebruiker niet voldoende bevoegd is voor het uitvoeren van de aanvraag of de gebruiker geen licentie heeft voor de gegevens die worden geopend. Alleen gebruikers met de vereiste machtigingen of licenties kunnen de aanvraag succesvol indienen.

**403 niet toegestaan: de juiste resource-API is geselecteerd.**

API-services zoals Microsoft Graph Controleer of de AUD claim (doelgroep) in het ontvangen toegangstoken overeenkomt met de waarde die wordt verwacht voor zichzelf, en zo niet, wordt de fout 403 niet toegestaan. Er is een veelvoorkomende fout opgetreden bij het gebruik van een token dat is verkregen voor Azure AD Graph-Api's, Outlook Api's of SharePoint/OneDrive-Api's voor het bellen van Microsoft Graph (of omgekeerd). Zorg ervoor dat de bronnen (of het bereik) van de app een token verkrijgen voor overeenkomsten met de API die de app aanroept.

**400 ongeldige aanvraag of 403 niet toegestaan: heeft de gebruiker naleven van de beleidsregels voor voorwaardelijke toegang van de organisatie?**

Een gebruiker die op basis van de beleidsregels van een organisatie de toegang krijgt tot Microsoft Graph-bronnen via de app kan worden aanvraagd voor aanvullende informatie die niet aanwezig is in het toegangstoken dat de app oorspronkelijk heeft aangeschaft. In dit geval ontvangt uw app een 400 met een *interaction_required* fout tijdens het verkrijgen van een toegangstoken of een 403 met *insufficient_claims* fout bij het bellen met Microsoft Graph. In beide gevallen bevat de fout respons aanvullende informatie die kan worden weergegeven aan het eindpunt voor de autorisatie van de gebruiker voor aanvullende informatie (zoals meervoudige verificatie of apparaatregistratie).

- [Voorwaarden voor voorwaardelijke toegang verwerken met MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Richtlijnen voor ontwikkelaars voor Azure Active Directory voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
