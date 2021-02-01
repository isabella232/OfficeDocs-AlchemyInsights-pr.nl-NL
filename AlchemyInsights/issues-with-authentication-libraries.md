---
title: Problemen met verificatiebibliotheken
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063604"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="7dfed-102">Problemen met verificatiebibliotheken</span><span class="sxs-lookup"><span data-stu-id="7dfed-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="7dfed-103">[In verificatiebibliotheken van Microsoft-identiteitsplatforms](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) worden door Microsoft ondersteunde en compatibele client- en middlewarebibliotheken vermeld.</span><span class="sxs-lookup"><span data-stu-id="7dfed-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="7dfed-104">De Microsoft Authentication Library (MSAL) ondersteunt verschillende [verificatiestromen](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) voor gebruik in verschillende toepassingsscenario's.</span><span class="sxs-lookup"><span data-stu-id="7dfed-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="7dfed-105">Als u tokens wilt verifiëren en verkrijgen, initialiseert u een nieuwe openbare of vertrouwelijke clienttoepassing in uw code.</span><span class="sxs-lookup"><span data-stu-id="7dfed-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="7dfed-106">U kunt verschillende configuratieopties instellen wanneer u de client-app initialiseert in de Microsoft Authentication Library (MSAL).</span><span class="sxs-lookup"><span data-stu-id="7dfed-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="7dfed-107">Zie de configuratieopties [voor toepassingen voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="7dfed-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="7dfed-108">**Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="7dfed-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7dfed-109">**Vanaf 30 juni 2020** voegen we geen nieuwe functies meer toe aan ADAL en Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="7dfed-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7dfed-110">We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.</span><span class="sxs-lookup"><span data-stu-id="7dfed-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7dfed-111">**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigen en bieden we geen technische ondersteuning of beveiligingsupdates meer.</span><span class="sxs-lookup"><span data-stu-id="7dfed-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7dfed-112">Apps met ADAL in bestaande besturingssysteemversies blijven werken na deze periode, maar krijgen geen technische *ondersteuning of beveiligingsupdates.*</span><span class="sxs-lookup"><span data-stu-id="7dfed-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="7dfed-113">Apps die na deze tijd Azure AD Graph gebruiken, ontvangen mogelijk geen reacties meer van het Azure AD Graph-eindpunt.</span><span class="sxs-lookup"><span data-stu-id="7dfed-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7dfed-114">**ADAL-migratie**</span><span class="sxs-lookup"><span data-stu-id="7dfed-114">**ADAL Migration**</span></span>

<span data-ttu-id="7dfed-115">U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.</span><span class="sxs-lookup"><span data-stu-id="7dfed-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7dfed-116">Als u Microsoft-apps gebruikt, weet u dat Microsoft voor het einde van de ondersteuningsdeadline haar toepassingen naar MSAL migreert, zodat ze kunnen profiteren van de lopende beveiligings- en functieverbeteringen van MSAL.</span><span class="sxs-lookup"><span data-stu-id="7dfed-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="7dfed-117">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="7dfed-117">For more information, see:</span></span>

1. [<span data-ttu-id="7dfed-118">Lees de veelgestelde vragen over ADAL</span><span class="sxs-lookup"><span data-stu-id="7dfed-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="7dfed-119">Meer informatie over het per platform migreren van apps</span><span class="sxs-lookup"><span data-stu-id="7dfed-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="7dfed-120">Als u hulp nodig hebt bij het gebruik van ADAL in uw apps, raden we u aan alle broncode van uw apps te controleren en, indien van toepassing, contact op te met alle ISV's of app-providers.</span><span class="sxs-lookup"><span data-stu-id="7dfed-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7dfed-121">Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="7dfed-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7dfed-122">**AAD Graph-migratie**</span><span class="sxs-lookup"><span data-stu-id="7dfed-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="7dfed-123">Voor toepassingen die gebruikmaken van Azure AD Graph volgt u onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="7dfed-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="7dfed-124">De controlelijst voor migratie biedt een beginpunt.</span><span class="sxs-lookup"><span data-stu-id="7dfed-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="7dfed-125">De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7dfed-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7dfed-126">Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers.</span><span class="sxs-lookup"><span data-stu-id="7dfed-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7dfed-127">Microsoft-ondersteuning kan u ook een lijst geven met alle AAD Graph-gebruik in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="7dfed-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="7dfed-128">De app heeft alleen toegang tot gegevens in Microsoft Graph als de gebruiker of beheerder de juiste machtigingen verleent via een toestemmingsproces.</span><span class="sxs-lookup"><span data-stu-id="7dfed-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7dfed-129">De [naslag voor Microsoft Graph-machtigingen](https://docs.microsoft.com/graph/permissions-reference) bevat de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft Graph-API's.</span><span class="sxs-lookup"><span data-stu-id="7dfed-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7dfed-130">Daarnaast vindt u hier richtlijnen voor het gebruik van de machtigingen.</span><span class="sxs-lookup"><span data-stu-id="7dfed-130">It also provides guidance about how to use the permissions.</span></span>
