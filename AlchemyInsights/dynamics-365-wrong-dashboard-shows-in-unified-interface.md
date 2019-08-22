---
title: Dynamics 365 - verkeerde Dashboard toont in Dynamics 365 eenduidige Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528546"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Verkeerde dashboard toont in Dynamics 365 eenduidige interface

Er zijn verschillende redenen waarom ziet u mogelijk een ander dashboard dan die u zou verwachten:

## <a name="the-user-has-set-a-user-default-dashboard"></a>De gebruiker heeft een gebruiker standaarddashboard instellen 

Meestal kunt u een gebruiker identificeren standaarddashboard is ingesteld als de knop **Als standaard instellen** niet op de opdrachtbalk dashboard weergegeven. De gebruiker standaarddashboard overschrijft alle andere standaard dashboards, zelfs als de gebruiker de standaarddashboard niet in de huidige app.

Gebruik de volgende tijdelijke oplossing uitschakelen hun standaarddashboard.

1. Maak een nieuw persoonlijk dashboard.

2. Die nieuwe dashboard instellen als de gebruikersstandaard.

3. Verwijder dit dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Het dashboard is ingesteld in de sitemap

U hebt een organisatie standaarddashboard ingesteld door het selecteren van een dashboard en 'Als standaard instellen' in het systeem aanpassen te kiezen. Maar het dashboard is gedefinieerd in de ontwerpfunctie van sitemap voorrang op dit dashboard, als de gebruiker toegang tot het heeft.

Als u wilt dat gebruikers toegang tot de dashboard die u hebt ingesteld als de Organisatiestandaard, kunt u:

* Stel dat dashboard in de sitemap

* Toegang tot het dashboard van de sitemap is gedefinieerd voor gebruikers verwijderen
