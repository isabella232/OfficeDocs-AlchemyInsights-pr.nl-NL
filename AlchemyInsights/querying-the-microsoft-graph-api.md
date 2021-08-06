---
title: Query's uitvoeren op de Microsoft Graph API
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923234"
---
# <a name="querying-the-microsoft-graph-api"></a>Query's uitvoeren op de Microsoft Graph API

Dit onderwerp kan ook van toepassing zijn op ontwikkelaars die nog steeds Azure AD Graph API. U wordt echter **ten zeerste** aangeraden Microsoft-Graph te gebruiken voor al uw adreslijst-, identiteits- en toegangsbeheerscenario's.

**Problemen met verificatie of autorisatie**

- Als uw  app geen tokens kan verkrijgen om Microsoft Graph te bellen, kiest u Probleem met het verkrijgen van een access **token (Authentication)** Microsoft Graph-categorie voor meer specifieke hulp en ondersteuning voor dit onderwerp.
- Als uw app **401 of 403** autorisatiefouten ontvangt bij het bellen van Microsoft Graph, kiest u de categorie Toegang geweigerde fout **(Autorisatie)** microsoft Graph API voor meer specifieke hulp en ondersteuning voor dit onderwerp.

**Ik wil Microsoft-Graph gebruiken, maar weet niet waar ik moet beginnen**

Zie het volgende voor meer informatie Graph Microsoft-Graph:

- [Overzicht van Microsoft-Graph](https://docs.microsoft.com/graph/overview)
- [Overzicht van identiteits- en accessbeheer in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Aan de slag met het bouwen Graph Microsoft-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Microsoft-Graph testen in uw tenant of een demo-tenant

**Ik wil Microsoft-Graph gebruiken, maar ondersteunt het de v1.0 directory-API's die ik nodig heb?**

Microsoft Graph is de aanbevolen API voor adreslijst-, identiteits- en toegangsbeheer. Er zijn echter nog enkele verschillen tussen wat er mogelijk is in Azure AD Graph en Microsoft Graph. Bekijk de volgende artikelen, waarin de meest recente verschillen worden belicht om u te helpen bij uw keuze:

- [Verschillen in resourcetype tussen Azure AD-Graph en Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschappenverschillen tussen Azure AD-Graph en Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodeverschillen tussen Azure AD en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Wanneer ik een query op het *gebruikersobject* uitvoert, ontbreken veel van de eigenschappen ervan**

`GET https://graph.microsoft.com/v1.0/users`retourneert alleen 11 eigenschappen, omdat Microsoft Graph automatisch een  standaardset gebruikerseigenschappen selecteert die u wilt retourneren. Als u andere *gebruikerseigenschappen nodig* hebt, gebruikt u $select om de eigenschappen te kiezen die uw toepassing nodig heeft. Probeer het eerst in **Microsoft Graph Explorer.**

**Sommige eigenschappen van gebruikers zijn *null,* ook al weet ik dat ze zijn ingesteld**

De meest waarschijnlijke verklaring is dat aan de toepassing de machtiging *User.ReadBasic.All is* verleend. Hierdoor kan de toepassing een beperkt aantal gebruikerseigenschappen lezen, waarbij alle andere eigenschappen als null worden geretourneerd, zelfs als ze eerder zijn ingesteld. Probeer in plaats daarvan de machtiging *User.Read.All* te verlenen.

Zie Microsoft Graph [gebruikersmachtigingen voor meer informatie.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Ik heb problemen met het gebruik van OData-queryparameters om gegevens in mijn aanvragen te filteren**

Hoewel Microsoft Graph een groot aantal OData-queryparameters ondersteunt, worden veel van deze parameters niet volledig ondersteund door adreslijstservices (bronnen die overnemen van *directoryObject)* in Microsoft Graph. Dezelfde beperkingen die aanwezig waren in Azure AD Graph blijven voor het grootste deel in Microsoft Graph:

1. **Niet ondersteund:**$count, $search en $filter  *null-waarden*
2. **Niet ondersteund:**$filter op bepaalde eigenschappen (zie resourceonderwerpen waarop eigenschappen kunnen worden gefilterd)
3. **Niet ondersteund:** pagineren, filteren en sorteren tegelijk
4. **Niet ondersteund:** filteren op een relatie. Zoek bijvoorbeeld alle leden van de technische groep die zich in het Verenigd Koninkrijk hebben.
5. **Gedeeltelijke ondersteuning:**$orderby *op gebruiker* (alleen displayName en userPrincipalName) en *groep*
6. Gedeeltelijke **ondersteuning:**$filter (ondersteunt alleen eq  *,* begint *met* of , en beperkt) ondersteuning, $expand (het uitbreiden van de relaties van één object retourneert alle relaties, maar het uitbreiden van een verzameling objectenrelaties is beperkt) 

Zie Reacties aanpassen [met queryparameters voor](https://docs.microsoft.com/graph/query-parameters)meer informatie.

**De API die ik bel werkt niet, waar kan ik meer testen?**

**Microsoft Graph Explorer-** Test Microsoft Graph API's in uw tenant of een demoten tenant en bekijk ook de voorbeeldquery's **in** Microsoft Graph Explorer.

**Wanneer ik gegevens opvraag, lijkt het alsof ik een onvolledige gegevensset terug krijg**

Als u een verzameling query's uitvoert (zoals *gebruikers),* gebruikt Microsoft Graph paginalimieten aan de serverzijde, zodat resultaten altijd worden geretourneerd met een standaardpaginaformaat. Uw app moet altijd verwachten dat u door verzamelingen gaat die zijn geretourneerd uit de service.

Zie voor meer informatie:

- [Microsoft Graph best practices](https://docs.microsoft.com/graph/best-practices-concept)
- [Gegevens van Microsoft Graph in uw app](https://docs.microsoft.com/graph/paging)

**Mijn app is te traag en wordt ook beperkt. Welke verbeteringen kan ik aanbrengen?**

Afhankelijk van uw scenario zijn er verschillende opties beschikbaar om uw toepassing performanter te maken en in sommige gevallen minder geneigd te worden beperkt door de service (wanneer u te veel gesprekken voert).

Hier vindt u meer informatie:

- [Microsoft Graph best practices](https://docs.microsoft.com/graph/best-practices-concept)
- [Batching requests](https://docs.microsoft.com/graph/json-batching)
- [Wijzigingen bijhouden via deltaquery](https://docs.microsoft.com/graph/delta-query-overview)
- [Ontvang een melding van wijzigingen via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Richtlijnen voor beperking](https://docs.microsoft.com/graph/throttling)

**Waar vind ik meer informatie over fouten en bekende problemen?**

- [Microsoft Graph foutreactiegegevens](https://docs.microsoft.com/graph/errors)
- [Bekende problemen met Microsoft-Graph](https://docs.microsoft.com/graph/known-issues)

**Waar kan ik de status van de beschikbaarheid en connectiviteit van de service controleren?**

De beschikbaarheid en connectiviteit van de onderliggende services die via Microsoft-Graph kunnen worden gebruikt, kunnen van invloed zijn op de algehele beschikbaarheid en prestaties van Microsoft Graph.

- Voor Azure Active Directory servicestatus controleert u de status van **beveiligings- en identiteitsservices** die worden vermeld op de [pagina Azure-status.](https://azure.microsoft.com/status/)
- Voor Office services die bijdragen aan Microsoft-Graph, controleert u de status van services die worden vermeld in [het Office Servicestatusdashboard.](https://portal.office.com/adminportal/home#/servicehealth)
