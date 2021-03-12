---
title: Problemen met OIDC-gebaseerde naadloze eenmalige aanmelding (SSO) oplossen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743973"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Problemen met OIDC-gebaseerde naadloze eenmalige aanmelding (SSO) oplossen

- Zie [Quickstart: Set up OIDC-based single sign-on (SSO) for an application in your Azure Active Directory (Azure AD) tenant (OIDC-based single sign-on( SSO) (OIDC-gebaseerde](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)app) aan uw Azure Active Directory-tenant (Azure AD) voor meer informatie over het toevoegen van een op OIDC gebaseerde app aan uw Azure Active Directory-tenant.
- Zie Één aanmelding op basis van OIDC begrijpen voor meer informatie over apps die de OpenID [Connect-standaard](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)gebruiken om één aanmelding te implementeren.
- Zie [OAuth 2.0- en OpenID Connect-protocollen op het Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)voor informatie als u ervoor kiest om uw code te schrijven door rechtstreeks HTTP-aanvragen te verzenden en af te handelen of een opensourcebibliotheek van derden te gebruiken in plaats van een van onze open-sourcebibliotheken te gebruiken.

**Protocollen**

1. [Microsoft identity platform and implicit grant flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) - The defining characteristic of the implicit grant is that tokens (ID tokens or access tokens) are returned directly from the /authorize endpoint instead of the /token endpoint. Dit wordt vaak gebruikt als onderdeel van de autorisatiecodestroom, in wat de **'hybride stroom'** wordt genoemd: het id-token ophalen op de aanvraag /autorisatie samen met een autorisatiecode. In dit artikel wordt beschreven hoe u rechtstreeks kunt programmeren tegen het protocol in uw toepassing om tokens aan te vragen bij Azure AD.
2. [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - The OAuth 2.0 authorization code grant can be used in apps that are installed on a device to gain access to protected resources, such as web APIIs. Met de implementatie van het Microsoft-identiteitsplatform van OAuth 2.0 kunt u aanmeldings- en API-toegang toevoegen aan uw mobiele en **desktop-apps.** In dit artikel wordt beschreven hoe u rechtstreeks tegen het protocol in uw toepassing kunt programmeren met elke taal.
3. [Microsoft-identiteitsplatform en OpenID Connect-protocol:](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) wanneer u de implementatie van OpenID Connect van het Microsoft-identiteitsplatform gebruikt, kunt u aanmeldings- en API-toegang toevoegen aan uw apps. In dit artikel wordt beschreven hoe u dit kunt doen onafhankelijk van taal en hoe u HTTP-berichten kunt verzenden en ontvangen zonder dat er **opensourcebibliotheken van Microsoft worden gebruikt.**
4. [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - You can use the OAuth 2.0 client credentials grantd specificd in RFC 6749, sometimes called **two-legged OAuth**, to access web-hosted resources by using the identity of an application. Dit type beurs wordt vaak gebruikt voor server-naar-server-interacties die op de achtergrond moeten worden uitgevoerd, zonder directe interactie met een gebruiker. Deze typen toepassingen worden vaak **daemons** of **serviceaccounts genoemd.** In dit artikel wordt beschreven hoe u rechtstreeks kunt programmeren tegen het protocol in uw toepassing.
