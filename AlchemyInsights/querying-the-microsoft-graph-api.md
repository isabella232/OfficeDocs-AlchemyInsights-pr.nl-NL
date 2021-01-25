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
# <a name="querying-the-microsoft-graph-api"></a>Een query uitvoeren op de Microsoft Graph-API

Dit onderwerp is mogelijk ook van toepassing op ontwikkelaars die gebruikmaken van Azure AD Graph API. Het wordt **ten zeerste** aanbevolen dat u Microsoft Graph gebruikt voor al uw adreslijst, identiteit en toegangsbeheer scenario's.

**Verificatie-of autorisatie problemen**

- Als het **niet lukt om** Microsoft Graph te bellen met de app, kiest u **probleem met het verkrijgen van een toegangstoken (Authentication)** Microsoft Graph-categorie voor een specifiekere Help en ondersteuning voor dit onderwerp.
- Als in uw app **401-of 403-autorisatiefouten** worden weergegeven bij het bellen van Microsoft Graph, kiest u de categorie **een fout bij het openen van een Access-fout (autorisatie)** bij het openen van een Microsoft Graph API-categorie voor een specifiekere Help en ondersteuning.

**Ik wil Microsoft Graph gebruiken, maar weet niet zeker waar u moet beginnen**

Zie voor meer informatie over Microsoft Graph:

- [Overzicht van Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Overzicht van identiteit en toegangsbeheer in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Aan de slag met Microsoft Graph-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -Api's Microsoft Graph testen in uw Tenant of een demo Tenant

**Ik wil Microsoft Graph gebruiken, maar biedt wel ondersteuning voor de v 1.0 Directory-Api's die ik nodig heb?**

Microsoft Graph is de aanbevolen API voor Directory, identiteit en toegangsbeheer. De mogelijkheden van Azure AD Graph en Microsoft Graph bestaan echter nog maar een paar hiaten. Lees de volgende artikelen om de meest recente verschillen te markeren om uw keuze te helpen:

- [Verschillen in brontype tussen Azure AD Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschappen verschillen tussen Azure AD Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methode verschillen tussen Azure AD en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Wanneer ik een query in het *gebruikers* object krijg, ontbreken een aantal eigenschappen**

`GET https://graph.microsoft.com/v1.0/users` Hiermee worden alleen 11 eigenschappen geretourneerd, omdat Microsoft Graph automatisch een standaardreeks *gebruikers* eigenschappen selecteert om te retourneren. Als u andere *gebruikers* eigenschappen nodig hebt, gebruikt u $SELECT om de eigenschappen te kiezen die de toepassing nodig heeft. Probeer het eerst in **Microsoft Graph Explorer** .

**Sommige waarden van gebruikerseigenschappen zijn *Null* , hoewel ik weet dat ze zijn ingesteld**

De meest waarschijnlijke uitleg is dat de toepassing de machtiging *User. ReadBasic. all* heeft gekregen. Hiermee kan de toepassing een beperkte set gebruikerseigenschappen lezen en alle andere eigenschappen als null terugzetten, zelfs als deze eerder zijn ingesteld. Probeer de toepassing *User. all. all* te verlenen.

Zie [gebruikersmachtigingen in Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions)voor meer informatie.

**Ik ondervind problemen bij het gebruik van OData-queryparameters om gegevens in mijn aanvragen te filteren**

Hoewel Microsoft Graph een groot aantal van de OData-queryparameters ondersteunt, worden veel van deze parameters niet volledig ondersteund door adreslijstservices (bronnen die gegevens overnemen van *directoryObject*) in Microsoft Graph. De beperkingen die aanwezig waren in azure AD Graph blijven voor het meeste deel in Microsoft Graph:

1. **Niet ondersteund**: $count, $search en $filter voor *Null* -of *niet-null* -waarden
2. **Niet ondersteund**: Hiermee $filter u op bepaalde eigenschappen (Zie de onderwerpen van bronnen over welke eigenschappen kunnen worden gefilterd)
3. **Niet ondersteund**: tegelijk pagineren, filteren en sorteren
4. **Niet ondersteund**: filteren op een relatie. Als u bijvoorbeeld alle leden van de technische groep in het VK wilt vinden.
5. **Gedeeltelijke ondersteuning**: $OrderBy op *gebruikers* (alleen naam en userPrincipalName) en *groep*
6. **Gedeeltelijke ondersteuning**: $filter (alleen ondersteuning voor *EQ*, *startsWith*, *of*, *en* *beperkte en* beperkte) ondersteuning, $expand (de relaties van één object uitvouwen, worden alle relaties geretourneerd, maar het uitvouwen van een verzameling objecten relaties is beperkt)

Zie [antwoorden aanpassen met queryparameters](https://docs.microsoft.com/graph/query-parameters)voor meer informatie.

**De API die ik bel, werkt niet; waar kan ik meer testen?**

**Microsoft Graph Explorer** -Microsoft Graph-api's testen in uw Tenant of een demo Tenant en ook de **Voorbeeldquery's** in Microsoft Graph Verkenner raadplegen.

**Wanneer ik een query voor de gegevens Zoek, lijkt het alsof ik een niet-voltooide gegevensverzameling weer**

Als u een query uitvoert op een verzameling (zoals *gebruikers*), worden in Microsoft Graph pagina limieten voor pagina's gebruikt, zodat resultaten altijd met een standaardpagina formaat worden geretourneerd. De verzameling die wordt geretourneerd door de service, moet altijd aan de app worden doorlopen.

Zie voor meer informatie:

- [Best practices voor Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Gegevens van Microsoft Graph in de app gepagineerd](https://docs.microsoft.com/graph/paging)

**Mijn app is te traag en wordt ook vertraagd. Welke verbeteringen kan ik aanbrengen?**

Afhankelijk van uw scenario zijn er verschillende opties voor de verwijdering, zodat de toepassing langer presteert en in sommige gevallen minder gevoelig is voor het beperken van de service (wanneer u te veel oproepen doet).

Hier vindt u meer informatie:

- [Best practices voor Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchaanvragen](https://docs.microsoft.com/graph/json-batching)
- [Wijzigingen bijhouden via een Delta query](https://docs.microsoft.com/graph/delta-query-overview)
- [Meldingen ontvangen over wijzigingen via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Richtlijnen voor beperken](https://docs.microsoft.com/graph/throttling)

**Waar vind ik meer informatie over fouten en bekende problemen?**

- [Informatie over fout antwoorden in Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Bekende problemen met Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Waar kan ik de status van de beschikbaarheid van de service en de verbinding controleren?**

De beschikbaarheid van de service en de verbinding van de onderliggende services die toegankelijk zijn via Microsoft Graph, kunnen de algehele beschikbaarheid en prestaties van Microsoft Graph beïnvloeden.

- Voor de status van Azure Active Directory-service controleert u de status van **Security + Identity** services die op de [pagina Azure status](https://azure.microsoft.com/status/)wordt weergegeven.
- Voor Office-services die bijdragen aan Microsoft Graph, controleert u de status van de services die worden vermeld in het [Dashboard Office service status](https://portal.office.com/adminportal/home#/servicehealth).
