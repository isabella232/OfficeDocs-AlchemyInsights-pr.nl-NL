---
title: Problemen met Microsoft Graph API
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713700"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="346f4-102">Problemen met Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="346f4-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="346f4-103">Dit onderwerp is mogelijk ook van toepassing op ontwikkelaars die nog steeds Azure AD Graph API gebruiken.</span><span class="sxs-lookup"><span data-stu-id="346f4-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="346f4-104">Het wordt echter **ten zeerste** aanbevolen Microsoft Graph te gebruiken voor al uw adreslijst-, identiteits- en toegangsbeheerscenario's.</span><span class="sxs-lookup"><span data-stu-id="346f4-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="346f4-105">**Verificatie- of autorisatieproblemen**</span><span class="sxs-lookup"><span data-stu-id="346f4-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="346f4-106">Als uw  app geen tokens kan verkrijgen om Microsoft Graph te bellen, kiest u Probleem met het verkrijgen van een Categorie voor toegangstoken **(Verificatie)** Microsoft Graph voor specifiekere hulp en ondersteuning voor dit onderwerp.</span><span class="sxs-lookup"><span data-stu-id="346f4-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="346f4-107">Als uw app **401-** of 403-autorisatiefouten ontvangt bij het bellen van Microsoft Graph, kiest u de categorie Microsoft Graph API (Getting an access denied **error) voor** specifieke hulp en ondersteuning voor dit onderwerp.</span><span class="sxs-lookup"><span data-stu-id="346f4-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="346f4-108">**Ik wil Microsoft Graph gebruiken, maar ik weet niet zeker waar ik moet beginnen**</span><span class="sxs-lookup"><span data-stu-id="346f4-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="346f4-109">Overzicht van Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="346f4-110">Overzicht van identiteits- en toegangsbeheer in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="346f4-111">Aan de slag met het maken van Microsoft Graph-apps</span><span class="sxs-lookup"><span data-stu-id="346f4-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="346f4-112">**Microsoft Graph Explorer** - Microsoft Graph-API's testen in uw tenant of een demo-tenant</span><span class="sxs-lookup"><span data-stu-id="346f4-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="346f4-113">**Ik wil Microsoft Graph gebruiken, maar ondersteunt het de v1.0-adreslijst-API's die ik nodig heb?**</span><span class="sxs-lookup"><span data-stu-id="346f4-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="346f4-114">Microsoft Graph is de aanbevolen API voor adreslijst-, identiteits- en toegangsbeheer.</span><span class="sxs-lookup"><span data-stu-id="346f4-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="346f4-115">Er zijn echter nog steeds een paar hiaten tussen wat mogelijk is in Azure AD Graph en Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="346f4-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="346f4-116">Bekijk de volgende artikelen, waarin de meest recente verschillen worden belicht die u moet helpen bij uw keuze:</span><span class="sxs-lookup"><span data-stu-id="346f4-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="346f4-117">Verschillen in resourcetype tussen Azure AD Graph en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="346f4-118">Verschillen in eigenschap tussen Azure AD Graph en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="346f4-119">Methodeverschillen tussen Azure AD en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="346f4-120">**De API die ik bel werkt niet. Waar kan ik meer tests uitvoeren?**</span><span class="sxs-lookup"><span data-stu-id="346f4-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="346f4-121">**Microsoft Graph Explorer-** Test Microsoft Graph API's in uw tenant of een demoten tenant en bekijk ook de voorbeeldquery's **in** Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="346f4-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="346f4-122">**Mijn app is te traag en wordt vertraagd. Welke verbeteringen kan ik aanbrengen?**</span><span class="sxs-lookup"><span data-stu-id="346f4-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="346f4-123">Afhankelijk van uw scenario kunt u diverse opties kiezen om uw toepassing efficiënter te maken en om in sommige gevallen minder snel te worden beperkt door de service (wanneer u te veel oproepen doet).</span><span class="sxs-lookup"><span data-stu-id="346f4-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="346f4-124">Best practices voor Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="346f4-125">Batchingaanvragen</span><span class="sxs-lookup"><span data-stu-id="346f4-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="346f4-126">Wijzigingen bijhouden via deltaquery</span><span class="sxs-lookup"><span data-stu-id="346f4-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="346f4-127">Via webhoekken op de hoogte worden gesteld van wijzigingen</span><span class="sxs-lookup"><span data-stu-id="346f4-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="346f4-128">Richtlijnen voor beperken</span><span class="sxs-lookup"><span data-stu-id="346f4-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="346f4-129">**Waar vind ik meer informatie over fouten en bekende problemen?**</span><span class="sxs-lookup"><span data-stu-id="346f4-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="346f4-130">Informatie over Microsoft Graph-foutreactie</span><span class="sxs-lookup"><span data-stu-id="346f4-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="346f4-131">Bekende problemen met Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="346f4-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="346f4-132">**Waar kan ik de status van de beschikbaarheid en connectiviteit van de service controleren?**</span><span class="sxs-lookup"><span data-stu-id="346f4-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="346f4-133">De beschikbaarheid en connectiviteit van de onderliggende services die kunnen worden gebruikt via Microsoft Graph, kan van invloed zijn op de algehele beschikbaarheid en prestaties van Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="346f4-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="346f4-134">Controleer voor de servicestatus van Azure Active Directory de status van de beveiligings- en **identiteitsservices** die worden weergegeven op de [statuspagina van Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="346f4-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="346f4-135">Voor Office-services die bijdragen aan Microsoft Graph controleert u de status van de services die worden weergegeven in het [Dashboard voor servicestatus van Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="346f4-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="346f4-136">Microsoft Graph-autorisatiefouten kunnen het gevolg zijn van verschillende problemen, waarvan de meeste een 401- of 403-fout genereren.</span><span class="sxs-lookup"><span data-stu-id="346f4-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="346f4-137">Het volgende kan bijvoorbeeld leiden tot autorisatiefouten:</span><span class="sxs-lookup"><span data-stu-id="346f4-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="346f4-138">Onjuiste [verwervingsstromen van toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="346f4-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="346f4-139">Slecht geconfigureerde [machtigingsbereiken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="346f4-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="346f4-140">Geen [toestemming](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="346f4-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="346f4-141">\**_Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="346f4-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="346f4-142">_*Vanaf 30 juni 2020*\* voegen we geen nieuwe functies meer toe aan ADAL en Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="346f4-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="346f4-143">We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.</span><span class="sxs-lookup"><span data-stu-id="346f4-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="346f4-144">**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigen en bieden we geen technische ondersteuning of beveiligingsupdates meer.</span><span class="sxs-lookup"><span data-stu-id="346f4-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="346f4-145">Apps met ADAL in bestaande besturingssysteemversies blijven werken na deze periode, maar krijgen geen technische *ondersteuning of beveiligingsupdates.*</span><span class="sxs-lookup"><span data-stu-id="346f4-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="346f4-146">Apps die na deze tijd Azure AD Graph gebruiken, ontvangen mogelijk geen reacties meer van het Azure AD Graph-eindpunt.</span><span class="sxs-lookup"><span data-stu-id="346f4-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="346f4-147">**ADAL-migratie**</span><span class="sxs-lookup"><span data-stu-id="346f4-147">**ADAL Migration**</span></span>

<span data-ttu-id="346f4-148">U wordt aangeraden bij te werken naar [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), dat de nieuwste functies en beveiligingsupdates bevat.</span><span class="sxs-lookup"><span data-stu-id="346f4-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="346f4-149">Als u Microsoft-apps gebruikt, weet u dat Microsoft voor het einde van de ondersteuningsdeadline haar toepassingen naar MSAL migreert, zodat ze kunnen profiteren van de lopende beveiligings- en functieverbeteringen van MSAL.</span><span class="sxs-lookup"><span data-stu-id="346f4-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="346f4-150">Lees de veelgestelde vragen over ADAL</span><span class="sxs-lookup"><span data-stu-id="346f4-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="346f4-151">Meer informatie over het per platform migreren van apps</span><span class="sxs-lookup"><span data-stu-id="346f4-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="346f4-152">Als u hulp nodig hebt bij het gebruik van ADAL in uw apps, raden we u aan alle broncode van uw apps te bekijken en, indien van toepassing, contact op te met alle ISV's of app-providers.</span><span class="sxs-lookup"><span data-stu-id="346f4-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="346f4-153">Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="346f4-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="346f4-154">**AAD Graph-migratie**</span><span class="sxs-lookup"><span data-stu-id="346f4-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="346f4-155">Voor toepassingen die Gebruikmaken van Azure AD Graph volgt u onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="346f4-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="346f4-156">[De controlelijst voor migratie biedt een beginpunt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="346f4-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="346f4-157">De registratieportal van uw Azure-app laat zien welke toepassingen gebruikmaken van AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="346f4-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="346f4-158">Het is raadzaam om alle broncodes van uw apps door te lezen en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers of app-providers.</span><span class="sxs-lookup"><span data-stu-id="346f4-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="346f4-159">Microsoft-ondersteuning kan u ook een lijst geven met alle AAD Graph-gebruik in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="346f4-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="346f4-160">De app heeft alleen toegang tot gegevens in Microsoft Graph als de gebruiker of beheerder de juiste machtigingen verleent via een toestemmingsproces.</span><span class="sxs-lookup"><span data-stu-id="346f4-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="346f4-161">De [microsoft Graph-machtigingenverwijzing bevat](https://docs.microsoft.com/graph/permissions-reference) de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft Graph-API's.</span><span class="sxs-lookup"><span data-stu-id="346f4-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="346f4-162">Daarnaast vindt u hier richtlijnen voor het gebruik van de machtigingen.</span><span class="sxs-lookup"><span data-stu-id="346f4-162">It also provides guidance about how to use the permissions.</span></span>
