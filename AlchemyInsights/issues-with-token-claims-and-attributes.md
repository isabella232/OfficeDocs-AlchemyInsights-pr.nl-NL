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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="07785-102">Problemen met tokenclaims en kenmerken</span><span class="sxs-lookup"><span data-stu-id="07785-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="07785-103">**Tokenclaims bijwerken, configureren of verwijderen**</span><span class="sxs-lookup"><span data-stu-id="07785-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="07785-104">Met behulp van Azure Active Directory (Azure AD) kunt u het [claimtype](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) voor de rolclaim aanpassen in het antwoord token dat u ontvangt nadat u een app hebt geautoriseerd.</span><span class="sxs-lookup"><span data-stu-id="07785-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="07785-105">Ontwikkelaars van toepassingen kunnen optionele claims in hun Azure AD-toepassingen gebruiken om op te geven welke claims ze willen gebruiken in tokens die naar hun toepassing worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="07785-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="07785-106">Zie Optionele claims [bij de app voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="07785-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="07785-107">[Groepsclaims configureren voor toepassingen met Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="07785-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="07785-108">Zie claims die zijn uitgegeven in het [SAML-token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)voor ondernemingstoepassingen als u naadloze eenpersoons aanmelden in uw toepassing gebruikt.</span><span class="sxs-lookup"><span data-stu-id="07785-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="07785-109">**Claims Attribute Mapping**</span><span class="sxs-lookup"><span data-stu-id="07785-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="07785-110">Zie Claims aanpassen die zijn weggelaten in tokens voor een specifieke app in een [tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)als u het toewijzingsbeleid voor claims wilt configureren met behulp van PowerShell.</span><span class="sxs-lookup"><span data-stu-id="07785-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="07785-111">Met de extensiekenmerken van het adreslijstschema kunt u aanvullende gegevens in Azure Active Directory opslaan op gebruikersobjecten en andere adreslijstobjecten, zoals groepen, tenantdetails en service-principals.</span><span class="sxs-lookup"><span data-stu-id="07785-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="07785-112">Alleen extensiekenmerken op gebruikersobjecten kunnen worden gebruikt voor niet-opeengebruikte claims in toepassingen.</span><span class="sxs-lookup"><span data-stu-id="07785-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="07785-113">[Als u extensiekenmerken voor adreslijstschema's gebruikt in claims,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) wordt beschreven hoe u de kenmerken van de extensie voor adreslijstschema's kunt gebruiken om gebruikersgegevens te verzenden naar toepassingen in tokenclaims.</span><span class="sxs-lookup"><span data-stu-id="07785-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="07785-114">Zie voor meer informatie over tokenclaims:</span><span class="sxs-lookup"><span data-stu-id="07785-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="07785-115">Claims in toegangstokens</span><span class="sxs-lookup"><span data-stu-id="07785-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="07785-116">Claims in een id_token</span><span class="sxs-lookup"><span data-stu-id="07785-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="07785-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) die u kunt verwachten in id-tokens en toegangstokens die zijn uitgegeven door Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="07785-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="07785-118">Verwijzing naar SAML-tokenclaims</span><span class="sxs-lookup"><span data-stu-id="07785-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
