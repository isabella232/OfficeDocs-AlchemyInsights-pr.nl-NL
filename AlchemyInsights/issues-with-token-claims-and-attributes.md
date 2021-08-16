---
title: Problemen met tokenclaims en -kenmerken
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012879"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemen met tokenclaims en -kenmerken

**Tokenclaims bijwerken, configureren of verwijderen**

1. Met Azure Active Directory (Azure AD) kunt u het [claimtype](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) voor de rolclaim aanpassen in het antwoord-token dat u ontvangt nadat u een app hebt geautoriseerd.
2. Toepassingsontwikkelaars kunnen optionele claims in hun Azure AD-toepassingen gebruiken om op te geven welke claims ze willen in tokens die naar hun toepassing worden verzonden. Zie Optionele claims voor [uw app verstrekken voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Groepsclaims configureren voor toepassingen met Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Zie Claims die zijn uitgegeven in het [SAML-token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)voor ondernemingstoepassingen aanpassen als u naadloze een-op-een-aanmelding in uw toepassing gebruikt.

**Toewijzing van claimskenmerk**

1. Zie Claims in tokens aanpassen voor een specifieke [app in een tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)als u het claimtoewijzingsbeleid wilt configureren met PowerShell.
2. Adreslijstschemaextensiekenmerken bieden een manier om extra gegevens op te slaan in Azure Active Directory gebruikersobjecten en andere adreslijstobjecten, zoals groepen, tenantdetails, service-principals. Alleen extensiekenmerken op gebruikersobjecten kunnen worden gebruikt voor het uitstoten van claims naar toepassingen. [Met behulp van adreslijstschemaextensiekenmerken in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) wordt beschreven hoe u adreslijstschemaextensiekenmerken gebruikt voor het verzenden van gebruikersgegevens naar toepassingen in tokenclaims.

Zie voor meer informatie over tokenclaims:

- [Claims in toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Claims in een id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) die u kunt verwachten in id-tokens en toegangstokens uitgegeven door Azure AD B2C
- [VERWIJZING NAAR SAML-tokenclaims](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
