---
title: Problemen met tokenclaims en kenmerken
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035889"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemen met tokenclaims en kenmerken

**Tokenclaims bijwerken, configureren of verwijderen**

1. Met behulp van Azure Active Directory (Azure AD) kunt u het [claimtype](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) voor de rolclaim aanpassen in het antwoord token dat u ontvangt nadat u een app hebt geautoriseerd.
2. Ontwikkelaars van toepassingen kunnen optionele claims in hun Azure AD-toepassingen gebruiken om op te geven welke claims ze willen gebruiken in tokens die naar hun toepassing worden verzonden. Zie Optionele claims [bij de app voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Groepsclaims configureren voor toepassingen met Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Zie claims die zijn uitgegeven in het [SAML-token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)voor ondernemingstoepassingen als u naadloze eenpersoons aanmelden in uw toepassing gebruikt.

**Claims Attribute Mapping**

1. Zie Claims aanpassen die zijn weggelaten in tokens voor een specifieke app in een [tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)als u het toewijzingsbeleid voor claims wilt configureren met behulp van PowerShell.
2. Met de extensiekenmerken van het adreslijstschema kunt u aanvullende gegevens in Azure Active Directory opslaan op gebruikersobjecten en andere adreslijstobjecten, zoals groepen, tenantdetails en service-principals. Alleen extensiekenmerken op gebruikersobjecten kunnen worden gebruikt voor niet-opeengebruikte claims in toepassingen. [Als u extensiekenmerken voor adreslijstschema's gebruikt in claims,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) wordt beschreven hoe u de kenmerken van de extensie voor adreslijstschema's kunt gebruiken om gebruikersgegevens te verzenden naar toepassingen in tokenclaims.

Zie voor meer informatie over tokenclaims:

- [Claims in toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Claims in een id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) die u kunt verwachten in id-tokens en toegangstokens die zijn uitgegeven door Azure AD B2C
- [Verwijzing naar SAML-tokenclaims](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
