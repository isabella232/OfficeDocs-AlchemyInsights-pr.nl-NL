---
title: SAML-bevestigingen (tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884983"
---
# <a name="saml-assertions-tokens"></a>SAML-bevestigingen (tokens)

1. SAML-tokens (Security Assertion Markup Language) zijn XML-weergaven van claims. Standaard worden SAML-tokens voor Windows Communication Foundation (WCF) in federatieve beveiligings scenario's uitgegeven tokens. Zie [SAML-tokens en claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)voor meer informatie.
2. Het Microsoft-identiteits platform laat verschillende typen beveiligingstokens voor de verwerking van elke verificatie stroom doen. Voor een [overzicht van SAML-token claims](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) worden de notatie, de beveiligingskenmerken en de inhoud van de SAML 2,0-tokens beschreven.
3. Volg de richtlijnen van de [levensduur van configureerbare tokens in Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) om inzicht te krijgen in het configureren van token levensduur.
4. Volg de stappen in [dit artikel](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) om inzicht te krijgen in de configuratie van Azure AD SAML-tokenversleuteling.
5. In azure AD kunt u opties instellen voor het ondertekenen van certificaten en de algoritme voor certificaatondertekening. Zie voor meer informatie [Geavanceerde opties voor certificaatondertekening in de SAML-token voor galerij-apps in azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
