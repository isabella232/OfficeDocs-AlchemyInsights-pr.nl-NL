---
title: Waarom is de knop budget toevoegen uitgeschakeld voor mij?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807280"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Waarom is de knop budget toevoegen uitgeschakeld voor mij?

Voor het maken van een budget hebt u een van de volgende machtigingen nodig:

- Beheergroep, abonnement, resource groepsbereik
- Inzender voor kostenbeheer
- Directeur
- Bent
- Alleen Enterprise Customer: inschrijving, afdeling, account bereik
- Registratie beheerder (budget instellen bij registratie bereik)
- Afdelings beheerder (budget instellen bij afdelings bereik)
- Account eigenaar (budget instellen bij account bereik)
- Alleen moderne klant overeenkomsten: factureringsrekening, facturerings profiel, bereik van factuur secties
- Azure abonnement Creator

**Ik heb een budget gemaakt wanneer mijn kosten voor de huidige maand al zijn budgetteren. Waarom heb ik geen meldingen ontvangen?**  
Als u al een bepaalde kosten drempel hebt overschreden wanneer u een budget maakt, wordt de waarschuwing niet geactiveerd. Wanneer een nieuwe cyclus begint, wordt de waarschuwing weergegeven als u de drempel niet ziet.

**Wanneer moet ik een melding verwachten wanneer ik een melding ontvang wanneer ik een van mijn gedefinieerde drempelwaarden voor budget meldingen heb overschreden?**  
Budgetten worden elke 4 uur geëvalueerd. Het duurt minimaal 8 uur voordat de gebruiksgegevens het budget stelsel bereiken. Dit kan waarschuwingen tot 12 uur duren nadat u een drempelwaarde hebt overschreden.

**Waarom is de knop begindatum uitgeschakeld wanneer ik een maand of een factureringsperiode voor maanden Selecteer?**  
Budgetten worden uitgelijnd op de huidige kalendermaand of de huidige factureringsperiode (in het geval waarin facturerings maand is geselecteerd). We vullen u daarom al deze waarde voor u in.

**Waarom zie ik geen grafiek van mijn kosten in de ervaring voor budget creatie?**  
We hebben minimaal twee maanden kostengegevens nodig voordat we een grafiek kunnen weergeven om u te helpen bij het maken van een budget.

**Waarom kan ik geen budget instellen voor een abonnement dat ik net heb gemaakt?**  
Nadat u een abonnement hebt gemaakt, duurt het 24-48 uur voordat de gegevens zijn gemaakt voor het uitvoeren van een budget.

**Bronnen voor budget-API**

- [Budget-API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): bewerkingen waarmee u budgetten kunt maken en bijwerken. Met behulp van de API budgetten kunt u een budgetdrempel instellen en meerdere waarschuwingen configureren om te worden geactiveerd wanneer u deze drempel aanpakt. Met waarschuwingen kan een e-mailbericht of een Azure-actiegroep worden geactiveerd om automatisering uit te voeren. Opmerking: het filteren van deze API is niet uitgelijnd met query-API filteren/dimensies.
- [Budget-API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Maak budgetten met een betere kosten filterfuncties dan v1. Filters worden uitgelijnd op het contract dat wordt gebruikt in onze query-en Dimension-Api's. Dit is de aanbevolen API voor budgetten voor het gebruik van forward.
- [Dimensies](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Hiermee kunt u bewerkingen uitvoeren om ondersteunde dimensies te krijgen voor uw gebruik in diverse bereiken. Met de Dimensions-API kunt u een lijst met dimensies ophalen die kunnen worden gebruikt als invoer voor het genereren van query's met de query-API.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): biedt bewerkingen om geaggregeerde kosten-en gebruiksgegevens te krijgen op basis van de query die u opgeeft. Met behulp van de query-API kunt u de gewenste filters, sortering en groepering voor alle beschikbare afmetingen opgeven (die worden geopend vanuit de Dimensions-API).

**Voorspelde kosten**

**Waarom zie ik geen prognoses voor mijn kosten in kostenanalyse?**  
Er zijn verschillende redenen waarom de prognose prognose voor u niet kan worden opgevolgd in kostenanalyse, een aantal van de volgende handelingen:

1. Als uw kostengegevens minder dan 10 dagen oud zijn, wordt de prognosegrafiek niet geladen. Voor het model zijn ten minste tien dagen recente kostengegevens vereist voor accurate projecties
2. Als u historische datums hebt geselecteerd, is de prognosegrafiek niet zichtbaar. Selecteer een datumbereik voor toekomstige datums waarop de prognosegrafiek moet worden weergegeven.
3. Als uw account meerdere valuta's bevat, wordt in de prognosegrafiek alleen de kosten project voor ' alle kosten in USD ' weergegeven.

**Waarom wordt de prognose niet gewijzigd als ik mijn resources Wijzig?**  
Voor het voorspellingsmodel zijn enkele dagen nodig om wijzigingen aan te brengen in het account en worden geen directe projecties gemaakt op basis van wijzigingen in resources.  
Voor grotere stappen voor het vergroten of verkleinen van de resources duurt het zo langer voordat deze wijzigingen zijn doorgevoerd in het account voor afwijkingen

**Waarom wordt mijn prognose versoepeld nadat ik de reservering of de verkoop van een marktplaats heb aangeschaft?**  
Het Prognosemodel beschouwt uw ' werkelijke kosten ' en is niet voor gebruik en aankoop apart. Voor een eenmalige aankoop verkleint het model de projecties na tien dagen om rekening te nemen met de plotselinge toename van de kosten

**Ik wil een prognose voor één dimensie zien (voorbeeld: Netwerk**  
Prognose biedt momenteel ondersteuning voor totale kostenprognoses en niet voor afzonderlijke meters. Wanneer ' gegroepeerd op ' een dimensie, zijn de projecties ook voor het totaal van alle items in de dimensie

**Aanbevolen documenten**

- [Wat is Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Best practices voor Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Uw kosten en uitgaven analyseren](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kosten verkennen en analyseren met kostenanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Beheer van Azure Cost: prijzen](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kosten controleren in kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video zelfstudie: een budget maken in de Azure-Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Vereisten voor het weergeven en aanpassen van budgetten](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budgetten maken en beheren](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatisering configureren met Azure-actiegroepen en budget-API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Gebruik kosten waarschuwingen om gebruik en uitgaven te bewaken](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Best practices voor kostenbeheer](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Zelfstudie Video's**

- [Een budget maken in de Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kosten beheren met de API en actiegroepen van de budgetten](https://go.microsoft.com/fwlink/?linkid=2147038)