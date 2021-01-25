---
title: Een query uitvoeren op de Microsoft Graph-API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974284"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="7d262-102">Een query uitvoeren op de Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="7d262-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="7d262-103">Dit onderwerp is mogelijk ook van toepassing op ontwikkelaars die gebruikmaken van Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="7d262-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="7d262-104">Het wordt **ten zeerste** aanbevolen dat u Microsoft Graph gebruikt voor al uw adreslijst, identiteit en toegangsbeheer scenario's.</span><span class="sxs-lookup"><span data-stu-id="7d262-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="7d262-105">**Verificatie-of autorisatie problemen**</span><span class="sxs-lookup"><span data-stu-id="7d262-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="7d262-106">Als het **niet lukt om** Microsoft Graph te bellen met de app, kiest u **probleem met het verkrijgen van een toegangstoken (Authentication)** Microsoft Graph-categorie voor een specifiekere Help en ondersteuning voor dit onderwerp.</span><span class="sxs-lookup"><span data-stu-id="7d262-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="7d262-107">Als in uw app **401-of 403-autorisatiefouten** worden weergegeven bij het bellen van Microsoft Graph, kiest u de categorie **een fout bij het openen van een Access-fout (autorisatie)** bij het openen van een Microsoft Graph API-categorie voor een specifiekere Help en ondersteuning.</span><span class="sxs-lookup"><span data-stu-id="7d262-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="7d262-108">**Ik wil Microsoft Graph gebruiken, maar weet niet zeker waar u moet beginnen**</span><span class="sxs-lookup"><span data-stu-id="7d262-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="7d262-109">Zie voor meer informatie over Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="7d262-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="7d262-110">Overzicht van Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="7d262-111">Overzicht van identiteit en toegangsbeheer in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="7d262-112">Aan de slag met Microsoft Graph-apps</span><span class="sxs-lookup"><span data-stu-id="7d262-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="7d262-113">**Microsoft Graph Explorer** -Api's Microsoft Graph testen in uw Tenant of een demo Tenant</span><span class="sxs-lookup"><span data-stu-id="7d262-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="7d262-114">**Ik wil Microsoft Graph gebruiken, maar biedt wel ondersteuning voor de v 1.0 Directory-Api's die ik nodig heb?**</span><span class="sxs-lookup"><span data-stu-id="7d262-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="7d262-115">Microsoft Graph is de aanbevolen API voor Directory, identiteit en toegangsbeheer.</span><span class="sxs-lookup"><span data-stu-id="7d262-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="7d262-116">De mogelijkheden van Azure AD Graph en Microsoft Graph bestaan echter nog maar een paar hiaten.</span><span class="sxs-lookup"><span data-stu-id="7d262-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="7d262-117">Lees de volgende artikelen om de meest recente verschillen te markeren om uw keuze te helpen:</span><span class="sxs-lookup"><span data-stu-id="7d262-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="7d262-118">Verschillen in brontype tussen Azure AD Graph en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="7d262-119">Eigenschappen verschillen tussen Azure AD Graph en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="7d262-120">Methode verschillen tussen Azure AD en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="7d262-121">**Wanneer ik een query in het *gebruikers* object krijg, ontbreken een aantal eigenschappen**</span><span class="sxs-lookup"><span data-stu-id="7d262-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="7d262-122">`GET https://graph.microsoft.com/v1.0/users` Hiermee worden alleen 11 eigenschappen geretourneerd, omdat Microsoft Graph automatisch een standaardreeks *gebruikers* eigenschappen selecteert om te retourneren.</span><span class="sxs-lookup"><span data-stu-id="7d262-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="7d262-123">Als u andere *gebruikers* eigenschappen nodig hebt, gebruikt u $SELECT om de eigenschappen te kiezen die de toepassing nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="7d262-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="7d262-124">Probeer het eerst in **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="7d262-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="7d262-125">**Sommige waarden van gebruikerseigenschappen zijn *Null* , hoewel ik weet dat ze zijn ingesteld**</span><span class="sxs-lookup"><span data-stu-id="7d262-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="7d262-126">De meest waarschijnlijke uitleg is dat de toepassing de machtiging *User. ReadBasic. all* heeft gekregen.</span><span class="sxs-lookup"><span data-stu-id="7d262-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="7d262-127">Hiermee kan de toepassing een beperkte set gebruikerseigenschappen lezen en alle andere eigenschappen als null terugzetten, zelfs als deze eerder zijn ingesteld.</span><span class="sxs-lookup"><span data-stu-id="7d262-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="7d262-128">Probeer de toepassing *User. all. all* te verlenen.</span><span class="sxs-lookup"><span data-stu-id="7d262-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="7d262-129">Zie [gebruikersmachtigingen in Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7d262-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="7d262-130">**Ik ondervind problemen bij het gebruik van OData-queryparameters om gegevens in mijn aanvragen te filteren**</span><span class="sxs-lookup"><span data-stu-id="7d262-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="7d262-131">Hoewel Microsoft Graph een groot aantal van de OData-queryparameters ondersteunt, worden veel van deze parameters niet volledig ondersteund door adreslijstservices (bronnen die gegevens overnemen van *directoryObject*) in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7d262-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="7d262-132">De beperkingen die aanwezig waren in azure AD Graph blijven voor het meeste deel in Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="7d262-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="7d262-133">**Niet ondersteund**: $count, $search en $filter voor *Null* -of *niet-null* -waarden</span><span class="sxs-lookup"><span data-stu-id="7d262-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="7d262-134">**Niet ondersteund**: Hiermee $filter u op bepaalde eigenschappen (Zie de onderwerpen van bronnen over welke eigenschappen kunnen worden gefilterd)</span><span class="sxs-lookup"><span data-stu-id="7d262-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="7d262-135">**Niet ondersteund**: tegelijk pagineren, filteren en sorteren</span><span class="sxs-lookup"><span data-stu-id="7d262-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="7d262-136">**Niet ondersteund**: filteren op een relatie.</span><span class="sxs-lookup"><span data-stu-id="7d262-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="7d262-137">Als u bijvoorbeeld alle leden van de technische groep in het VK wilt vinden.</span><span class="sxs-lookup"><span data-stu-id="7d262-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="7d262-138">**Gedeeltelijke ondersteuning**: $OrderBy op *gebruikers* (alleen naam en userPrincipalName) en *groep*</span><span class="sxs-lookup"><span data-stu-id="7d262-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="7d262-139">**Gedeeltelijke ondersteuning**: $filter (alleen ondersteuning voor *EQ*, *startsWith*, *of*, *en* *beperkte en* beperkte) ondersteuning, $expand (de relaties van één object uitvouwen, worden alle relaties geretourneerd, maar het uitvouwen van een verzameling objecten relaties is beperkt)</span><span class="sxs-lookup"><span data-stu-id="7d262-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="7d262-140">Zie [antwoorden aanpassen met queryparameters](https://docs.microsoft.com/graph/query-parameters)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7d262-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="7d262-141">**De API die ik bel, werkt niet; waar kan ik meer testen?**</span><span class="sxs-lookup"><span data-stu-id="7d262-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="7d262-142">**Microsoft Graph Explorer** -Microsoft Graph-api's testen in uw Tenant of een demo Tenant en ook de **Voorbeeldquery's** in Microsoft Graph Verkenner raadplegen.</span><span class="sxs-lookup"><span data-stu-id="7d262-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="7d262-143">**Wanneer ik een query voor de gegevens Zoek, lijkt het alsof ik een niet-voltooide gegevensverzameling weer**</span><span class="sxs-lookup"><span data-stu-id="7d262-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="7d262-144">Als u een query uitvoert op een verzameling (zoals *gebruikers*), worden in Microsoft Graph pagina limieten voor pagina's gebruikt, zodat resultaten altijd met een standaardpagina formaat worden geretourneerd.</span><span class="sxs-lookup"><span data-stu-id="7d262-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="7d262-145">De verzameling die wordt geretourneerd door de service, moet altijd aan de app worden doorlopen.</span><span class="sxs-lookup"><span data-stu-id="7d262-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="7d262-146">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="7d262-146">For more information, see:</span></span>

- [<span data-ttu-id="7d262-147">Best practices voor Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="7d262-148">Gegevens van Microsoft Graph in de app gepagineerd</span><span class="sxs-lookup"><span data-stu-id="7d262-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="7d262-149">**Mijn app is te traag en wordt ook vertraagd. Welke verbeteringen kan ik aanbrengen?**</span><span class="sxs-lookup"><span data-stu-id="7d262-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="7d262-150">Afhankelijk van uw scenario zijn er verschillende opties voor de verwijdering, zodat de toepassing langer presteert en in sommige gevallen minder gevoelig is voor het beperken van de service (wanneer u te veel oproepen doet).</span><span class="sxs-lookup"><span data-stu-id="7d262-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="7d262-151">Hier vindt u meer informatie:</span><span class="sxs-lookup"><span data-stu-id="7d262-151">To learn more, see:</span></span>

- [<span data-ttu-id="7d262-152">Best practices voor Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="7d262-153">Batchaanvragen</span><span class="sxs-lookup"><span data-stu-id="7d262-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="7d262-154">Wijzigingen bijhouden via een Delta query</span><span class="sxs-lookup"><span data-stu-id="7d262-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="7d262-155">Meldingen ontvangen over wijzigingen via webhooks</span><span class="sxs-lookup"><span data-stu-id="7d262-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="7d262-156">Richtlijnen voor beperken</span><span class="sxs-lookup"><span data-stu-id="7d262-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="7d262-157">**Waar vind ik meer informatie over fouten en bekende problemen?**</span><span class="sxs-lookup"><span data-stu-id="7d262-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="7d262-158">Informatie over fout antwoorden in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="7d262-159">Bekende problemen met Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d262-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="7d262-160">**Waar kan ik de status van de beschikbaarheid van de service en de verbinding controleren?**</span><span class="sxs-lookup"><span data-stu-id="7d262-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="7d262-161">De beschikbaarheid van de service en de verbinding van de onderliggende services die toegankelijk zijn via Microsoft Graph, kunnen de algehele beschikbaarheid en prestaties van Microsoft Graph beïnvloeden.</span><span class="sxs-lookup"><span data-stu-id="7d262-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="7d262-162">Voor de status van Azure Active Directory-service controleert u de status van **Security + Identity** services die op de [pagina Azure status](https://azure.microsoft.com/status/)wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="7d262-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="7d262-163">Voor Office-services die bijdragen aan Microsoft Graph, controleert u de status van de services die worden vermeld in het [Dashboard Office service status](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7d262-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
