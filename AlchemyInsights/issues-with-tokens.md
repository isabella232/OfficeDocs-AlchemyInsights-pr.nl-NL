---
title: Problemen met tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916845"
---
# <a name="issues-with-tokens"></a>Problemen met tokens

Als u problemen met tokens wilt beheren, kunt u de volgende stappen uitvoeren:

1. U kunt de levensduur opgeven van een toegang, ID of SAML-token die is uitgegeven door Microsoft Identity platform. U kunt token levensduur instellen voor alle apps in uw organisatie, voor een toepassing via meerdere tenants of voor een bepaalde service-principal in uw organisatie. Voor meer informatie raadpleegt u de [levensduur van configureerbare tokens in Microsoft Identity platform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Met behulp van toegangstokens kunnen clients beveiligde web-Api's aanroepen en worden deze gebruikt door Web-Api's om verificatie en autorisatie uit te voeren. Net als bij de OAuth-specificatie, zijn toegangstokens ondoorzichtige tekenreeksen zonder een indeling met bepaalde identiteitsproviders (IDPs) GUID'S, en anderen gebruiken versleutelde blob's. Met het Microsoft Identity platform wordt een groot aantal toegangstoken indelingen gebruikt, afhankelijk van de configuratie van de API die het token accepteert. Zie [toegangstokens voor Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)voor informatie over hoe uw API de claims binnen een toegangstoken kan valideren en gebruiken.
3. De Microsoft Authentication Library (MSAL) ondersteunt diverse verificatie stromen voor gebruik in verschillende toepassings scenario's. Zie [verificatie stromen](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)voor meer informatie.
4. De autorisatiecode voor OAuth 2,0 kan worden gebruikt in apps die zijn geïnstalleerd op een apparaat om toegang te krijgen tot beveiligde bronnen, zoals web-Api's. Met de implementatie van Microsoft Identity platform van OAuth 2,0, kunt u aanmelden en API-toegang voor uw mobiele en bureaubladtoepassingen toevoegen. Zie [Microsoft Identity platform en OAuth 2,0 Authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) voor het rechtstreeks uitvoeren van het protocol in uw toepassing, met behulp van een taal.
5. OpenID Connect (OIDC) is een Authenticatieprotocol op basis van OAuth 2,0, dat u kunt gebruiken om een gebruiker veilig aan te melden bij een toepassing. Wanneer u de implementatie van het Microsoft Identity platform-eindpunt voor OpenID Connect gebruikt, kunt u aanmelden en API-toegang voor uw apps toevoegen. [Microsoft Identity platform en OpenID Connect protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) toont de manier waarop u dit onafhankelijk van de taal kunt uitvoeren en hoe u HTTP-berichten verzendt en ontvangt zonder gebruik te maken van een Microsoft open-source-bibliotheek.
    - Het UserInfo-eindpunt maakt deel uit van de OIDC-standaard, ontworpen om claims te retourneren over de geverifieerde gebruiker. Zie voor meer informatie het [eindpunt van het Microsoft Identity platform userinfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Wanneer u [een web-API aanroept in een web-app met behulp van Azure AD en OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) , ziet u hoe u een MVC-webtoepassing maakt die gebruikmaakt van Azure AD voor aanmelding met behulp van het OpenID-verbindingsprotocol en vervolgens een web-API aanroept onder de identiteit van de aangemelde gebruiker met tokens die zijn verkregen via OAuth 2,0. In dit voorbeeld wordt de OpenID Connect ASP .net OWIN middleware en ADAL .net gebruikt.
6. [Een toepassing configureren voor](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) het weergeven van een web-API: in dit voorbeeld gebruik kunt u een web-API registreren met het Microsoft-identiteits platform en deze weergeven aan client-apps door een voorbeeld bereik toe te voegen. Als u uw web-API registreert en deze via scopes weergeeft, kunt u toegang verlenen tot de bronnen van gemachtigde gebruikers en client-apps die toegang hebben tot uw API.
7. In azure Active Directory B2C (Azure AD B2C) is de gebruikers stroom van de resource-eigenaar (ROPC) een OAuth-standaardverificatie stroom. In deze stroom is een toepassing, ook wel bekend als de Relying Party, geldige referenties voor tokens uitgewisseld. De referenties bevatten een gebruikers-ID en wachtwoord. De geretourneerde tokens zijn een ID-token, toegangstoken en een vernieuwingstoken. Zie voor meer informatie [de gebruikers stroom voor het wachtwoord van een resource-eigenaar instellen in azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

