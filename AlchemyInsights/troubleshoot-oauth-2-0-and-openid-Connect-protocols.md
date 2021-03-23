---
title: Problemen met OAuth 2.0 en OpenID Connect-protocollen oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035597"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Problemen met OAuth 2.0 en OpenID Connect-protocollen oplossen

Als u problemen met OAuth 2.0 en OpenID Connect wilt oplossen, voert u de volgende aanbevolen stappen uit:

Raadpleeg de volgende artikelen die betrekking hebben op het configureren en oplossen van problemen met OAuth 2.0- en OpenID Connect-protocollen:

- [Microsoft-identiteitsplatform en OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) autorisatiecodestroom : In dit artikel wordt beschreven hoe u rechtstreeks kunt programmeren tegen de **pkce-stroom (Code Grant)** in uw toepassing, met elke taal.
- [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - This article described how to program directly against the **client credentials flow** in your application.
- [Microsoft identity platform and OAuth 2.0 Resource Owner Password Credentials](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - In dit artikel wordt beschreven hoe u rechtstreeks kunt programmeren tegen de **ROPC-stroom** in uw toepassing.
    - Het Microsoft-identiteitsplatform ondersteunt alleen ROPC voor Azure AD-tenants en niet voor persoonlijke accounts. Dit betekent dat u een tenant-specifiek eindpunt **(of https://login.microsoftonline.com/{TenantId_or_Name})** het **eindpunt van de organisatie)** moet gebruiken.
    - Persoonlijke accounts die zijn uitgenodigd voor een Azure AD-tenant kunnen GEEN ROPC gebruiken.
    - Accounts die geen wachtwoord hebben, kunnen zich niet aanmelden via ROPC. Voor dit scenario raden we u aan in plaats daarvan een andere stroom voor uw app te gebruiken.
    - Als gebruikers meervoudige verificatie [(MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) moeten gebruiken om zich aan te melden bij de toepassing, worden ze geblokkeerd.
    - ROPC wordt niet ondersteund in scenario's voor hybride [identiteitsfederaties](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (bijvoorbeeld Azure AD en ADFS die worden gebruikt om on-premises accounts te verifiëren). Als gebruikers worden omgeleid naar een on-premises identiteitsprovider, kan Azure AD de gebruikersnaam en het wachtwoord niet testen op die identiteitsprovider. [Pass-throughverificatie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) wordt echter ondersteund met ROPC.
    - Een uitzondering op een scenario van een hybride identiteitsfederatie is het volgende: Met het beleid Voor het ontdekken van home realm met **AllowCloudPasswordValidation** ingesteld op **WAAR** kan de ROPC-stroom werken voor federatieve gebruikers wanneer on-premises wachtwoord wordt gesynchroniseerd met de cloud. Zie Directe [ROPC-verificatie](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) van federatief gebruikers inschakelen voor oudere toepassingen voor meer informatie. 
- [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - In dit artikel wordt beschreven hoe u rechtstreeks kunt programmeren op basis van de **OBO-stroom** in uw toepassing.
- [Microsoft-identiteitsplatform en OpenID Connect-protocol:](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) in dit artikel wordt beschreven hoe u het OpenID Connect-protocol kunt implementeren onafhankelijk van taal en hoe u HTTP-berichten kunt verzenden en ontvangen zonder dat er opensourcebibliotheken van Microsoft worden gebruikt.

**Toegangstokens**

[Toegangstokens voor microsoft-identiteitsplatform:](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) ontdek hoe uw API de claims in een toegangstoken kan valideren en gebruiken. Alle documentatie in dit artikel, behalve waar vermeld, is alleen van toepassing op tokens die zijn uitgegeven voor API's die u hebt geregistreerd. Het is niet van toepassing op tokens die zijn uitgegeven voor API's van Microsoft en deze tokens kunnen ook niet worden gebruikt om te valideren hoe het Microsoft-identiteitsplatform tokens uitdeelt voor een API die u maakt.

**Toepassingsconfiguratie**

Beperkingen en beperkingen voor omleiden van [URI (antwoord-URL)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Meer informatie over het configureren van uw Redirect URI (antwoord-URL). Een omleidings-URI of antwoord-URL is de locatie waar de autorisatieserver de gebruiker verzendt nadat de app is geautoriseerd en een autorisatiecode of toegangscode heeft verleend. De autorisatieserver verzendt de code of het token naar de omleidings-URI; het is dus belangrijk dat u de juiste locatie registreert als onderdeel van het registratieproces voor apps.

**Toepassingsbepaling**

[Zelfstudie: Inrichting](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) ontwikkelen en plannen voor een SCIM-eindpunt: in dit artikel wordt beschreven hoe u een SCIM-eindpunt kunt maken en kunt integreren met de AAD-inrichtingsservice.


