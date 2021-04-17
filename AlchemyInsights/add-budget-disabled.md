---
title: Waarom is de knop Budget toevoegen voor mij uitgeschakeld?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822630"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Waarom is de knop Budget toevoegen voor mij uitgeschakeld?

Als u een budget wilt maken, hebt u een van de volgende machtigingen nodig:

- Beheergroep, Abonnement, Resourcegroepbereiken
- Inzender kostenbeheer
- Eigenaar
- Inzender
- Alleen ondernemingsklant: inschrijving, afdeling, accountbereiken
- Inschrijvingsbeheerder (budget instellen bij inschrijvingsbereik)
- Afdelingsbeheerder (budget instellen op afdelingsbereik)
- Accounteigenaar (budget instellen op accountbereik)
- Alleen moderne klantovereenkomst: factureringsaccount, factureringsprofiel, sectiebereiken factuur
- Maker van Azure-abonnementen

**Ik heb een budget gemaakt toen mijn kosten voor de huidige maand al te veel waren. Waarom heb ik geen waarschuwing ontvangen?**  
Als u een bepaalde kostendrempel al hebt overschreden wanneer u een budget maakt dat niet wordt gealarmeerd. Wanneer een nieuwe cyclus begint, wordt de waarschuwing gestart als u de drempel overschrijdt.

**Wanneer verwacht ik een waarschuwing te ontvangen nadat ik een van mijn gedefinieerde drempelwaarden voor budgetwaarschuwingen heb overschreden?**  
Budgetten worden elke 4 uur geëvalueerd. Het duurt minimaal 8 uur voordat gebruiksgegevens het budgetsysteem hebben bereikt. Hierdoor kan het tot 12 uur duren voordat waarschuwingen worden afgestoken nadat u een drempel hebt overschreden.

**Waarom is de knop Begindatum uitgeschakeld wanneer ik een resetperiode van maand of factureringsmaand selecteer?**  
Budgetten worden uitgelijnd op de huidige kalendermaand of huidige factureringsperiode (in het geval dat Factureringsmaand is geselecteerd). Daarom vullen we deze waarde vooraf voor u in.

**Waarom zie ik geen grafiek van mijn kosten in de ervaring voor het maken van budgetten?**  
We hebben minimaal 2 maanden kostengegevens nodig voordat we een grafiek kunnen maken om u te helpen bij het maken van budgetten.

**Waarom kan ik geen budget instellen voor een abonnement dat ik zojuist heb gemaakt?**  
Na het maken van een abonnement duurt het 24-48 uur voordat u een budget instelt.

**Budget-API-resources**

- [Budgetten API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Biedt bewerkingen voor het maken en bijwerken van budgetten. Met de Budgetten-API kunt u een budgetdrempel instellen en meerdere waarschuwingen configureren voor brand wanneer u deze drempel nadert. Waarschuwingen kunnen een e-mail of een Azure-actiegroep activeren om automatisering uit te voeren. Opmerking: Filteren voor deze API wordt niet uitgelijnd met Query API-filtering /dimensies.
- [Budgetten API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Maak budgetten met meer mogelijkheden voor het filteren van kosten dan v1. Filteren wordt uitgelijnd op het contract dat wordt gebruikt in onze query- en dimensie-API's. Dit is de aanbevolen budgetten-API om vooruit te gaan.
- [Dimensies:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)biedt bewerkingen om ondersteunde dimensies te krijgen voor uw gebruik onder verschillende bereikmen. Met de Dimensions API kunt u een lijst met dimensies ophalen die kunnen worden gebruikt als input voor het genereren van query's met de Query-API.
- [Query:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Biedt bewerkingen voor het verzamelen van samengevoegde kosten- en gebruiksgegevens op basis van de query die u oplevert. Met behulp van de Query-API kunt u de gewenste filtering, sortering en groepering opgeven voor alle beschikbare dimensies (die toegankelijk zijn via de Dimensions API).

**Prognosekosten**

**Waarom zie ik geen prognoses voor mijn kosten in Kostenanalyse?**  
Er zijn meerdere redenen waarom de prognoseprognose voor u mogelijk ontbreekt in Kostenanalyse, sommige zijn als volgt:

1. Als uw kostengegevens minder dan 10 dagen oud zijn, wordt het prognosediagram niet geladen. Het model vereist ten minste 10 dagen recente kostengegevens voor nauwkeurige prognoses
2. Als u historische datums hebt geselecteerd, is het prognosediagram niet zichtbaar. Selecteer een datumbereik met toekomstige datums voor de prognosegrafiek die moet worden weergegeven
3. Als uw account meerdere valuta's heeft, worden in de prognosegrafiek alleen projectkosten gemaakt voor 'Alle kosten in USD'

**Waarom wordt de prognose niet gewijzigd wanneer ik wijzigingen aan mijn resources aan maak?**  
Het prognosemodel vereist een paar dagen om rekening te houden met wijzigingen in het account en maakt geen directe prognoses op basis van wijzigingen in resources  
Voor grotere stappen voor het vergroten of verminderen van resources duurt het iets langer om het model aan te passen aan deze wijzigingen om afwijkingen te verantwoorden

**Waarom wordt mijn prognose groter nadat ik een reservering heb gemaakt of marketplace heb gekocht?**  
In het prognosemodel wordt rekening gehouden met de werkelijke kosten en wordt het gebruik en de aankoop niet afzonderlijk verantwoord. Voor een eendaagse aankoop worden de prognoses na 10 dagen met het model verkleind om de plotse stijging van de kosten te verantwoorden

**Ik wil prognoses zien voor één dimensie (bijvoorbeeld. Meter)**  
Prognose ondersteunt momenteel de totale kostenprognoses en niet voor afzonderlijke meters. Wanneer een dimensie wordt gegroepeerd op, zijn de projecties dus voor het totaal van alle items in de dimensie

**Aanbevolen documenten**

- [Wat is Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Best practices voor Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Uw kosten en uitgaven analyseren](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kosten verkennen en analyseren met kostenanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Prijzen](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kosten controleren in kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videozelfstudie: Een budget maken in de Azure-portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Vereisten voor het weergeven en aanpassen van budgetten](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budgetten maken en beheren](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatisering configureren met Azure Action Groups and Budgets API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Kostenwaarschuwingen gebruiken om het gebruik en de uitgaven te controleren](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Best practices voor kostenbeheer](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Zelfstudievideo's**

- [Een budget maken in de Azure-portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kosten beheren met de Budgetten-API en Actiegroepen](https://go.microsoft.com/fwlink/?linkid=2147038)