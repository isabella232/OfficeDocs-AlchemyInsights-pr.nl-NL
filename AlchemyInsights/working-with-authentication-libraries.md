---
title: Werken met verificatiebibliotheken
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035287"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="da391-102">Werken met verificatiebibliotheken</span><span class="sxs-lookup"><span data-stu-id="da391-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="da391-103">Als u het msal-probleem (Microsoft Authentication Library) wilt oplossen, voert u de volgende aanbevolen stappen uit:</span><span class="sxs-lookup"><span data-stu-id="da391-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="da391-104">**Werken met MSAL:** [Verificatiebibliotheken van microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - In dit artikel wordt ondersteuning voor Microsoft Authentication Library voor verschillende toepassingstypen beschreven.</span><span class="sxs-lookup"><span data-stu-id="da391-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="da391-105">Het bevat koppelingen naar bibliotheekbroncode. waar u het pakket voor het project van uw app kunt downloaden; en of de bibliotheek gebruikers aanmelden (verificatie), toegang tot beveiligde web-API's (autorisatie) of beide ondersteunt.</span><span class="sxs-lookup"><span data-stu-id="da391-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="da391-106">**Verificatie oplossen:** MsAL ondersteunt verschillende verificatiestromen voor gebruik in verschillende toepassingsscenario's.</span><span class="sxs-lookup"><span data-stu-id="da391-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="da391-107">Afhankelijk van hoe uw clienttoepassing is gemaakt, kan msal een of meer verificatiestromen gebruiken die worden ondersteund door het Microsoft-identiteitsplatform.</span><span class="sxs-lookup"><span data-stu-id="da391-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="da391-108">Deze stromen kunnen verschillende typen tokens en autorisatiecodes produceren en vereisen verschillende tokens om ze te laten werken.</span><span class="sxs-lookup"><span data-stu-id="da391-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="da391-109">**Toegangstokens:** [Toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) voor microsoft-identiteitsplatform- Lees hoe uw API de claims in een toegangstoken kan valideren en gebruiken.</span><span class="sxs-lookup"><span data-stu-id="da391-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="da391-110">Alle documentatie in dit artikel, behalve waar vermeld, is alleen van toepassing op tokens die zijn uitgegeven voor API's die u hebt geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="da391-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="da391-111">Het is niet van toepassing op tokens die zijn uitgegeven voor API's van Microsoft en deze tokens kunnen ook niet worden gebruikt om te valideren hoe het Microsoft-identiteitsplatform tokens uitdeelt voor een API die u maakt.</span><span class="sxs-lookup"><span data-stu-id="da391-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="da391-112">**Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="da391-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="da391-113">**Vanaf 30 juni 2020** worden er geen nieuwe functies meer toegevoegd aan ADAL en Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="da391-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="da391-114">We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.</span><span class="sxs-lookup"><span data-stu-id="da391-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="da391-115">**Vanaf 30 juni 2022** beëindigen we de ondersteuning voor ADAL en Azure AD Graph en bieden we geen technische ondersteuning of beveiligingsupdates meer.</span><span class="sxs-lookup"><span data-stu-id="da391-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="da391-116">Apps die ADAL gebruiken voor bestaande besturingssysteemversies blijven na deze tijd werken, maar krijgen geen *technische ondersteuning of beveiligingsupdates.*</span><span class="sxs-lookup"><span data-stu-id="da391-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="da391-117">Apps met Azure AD Graph na deze periode ontvangen mogelijk geen antwoorden meer van het Azure AD Graph-eindpunt.</span><span class="sxs-lookup"><span data-stu-id="da391-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="da391-118">**ADAL-migratie**</span><span class="sxs-lookup"><span data-stu-id="da391-118">**ADAL Migration**</span></span>

- <span data-ttu-id="da391-119">We raden u aan bij te werken naar msal, met de nieuwste functies en beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="da391-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="da391-120">Als u Microsoft-apps gebruikt, weet dan dat Microsoft bezig is met het migreren van de apps naar MSAL tegen het einde van de ondersteuningsdeadline, zodat ze profiteren van de voortdurende beveiligings- en functieverbeteringen van MSAL.</span><span class="sxs-lookup"><span data-stu-id="da391-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="da391-121">[Lees de veelgestelde vragen over ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="da391-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="da391-122">[Meer informatie over het migreren van apps per platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="da391-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="da391-123">Als u na het lezen van de handleiding voor het platform van uw app aanvullende vragen hebt, kunt u een bericht plaatsen op [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) met de tag [azure-ad-adal-deprecation] of een probleem openen in de GitHub-opslagplaats van de bibliotheek.</span><span class="sxs-lookup"><span data-stu-id="da391-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="da391-124">Zie de [sectie Talen en frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) van het **MSAL-overzichtsartikel** voor koppelingen naar de repo van elke bibliotheek.</span><span class="sxs-lookup"><span data-stu-id="da391-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="da391-125">**Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL** wordt gebruikt, raden we u aan de broncode van al uw apps te controleren.</span><span class="sxs-lookup"><span data-stu-id="da391-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="da391-126">Indien van toepassing, kunt u contact op met onafhankelijke softwareleveranciers (ISV's) of app-providers.</span><span class="sxs-lookup"><span data-stu-id="da391-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="da391-127">Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="da391-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







