---
title: Dynamics 365-onjuist dashboard wordt weergegeven in Dynamics 365 unified interface
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528546"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Onjuist dashboard wordt weergegeven in Dynamics 365 unified interface

Er zijn verschillende redenen waarom u een ander Dashboard zien dan het overzicht dat u verwacht:

## <a name="the-user-has-set-a-user-default-dashboard"></a>De gebruiker heeft een standaarddashboard voor gebruikers ingesteld 

Meestal u een standaarddashboard van de gebruiker instellen als de knop **als standaard instellen** niet wordt weergegeven in de opdrachtbalk van het dashboard. Het standaarddashboard van de gebruiker overschrijft alle andere standaard dashboards, zelfs als het standaarddashboard van de gebruiker zich niet in de huidige app bevindt.

Gebruik de volgende oplossing om het standaarddashboard te ontkoppelen.

1. Maak een nieuw persoonlijk dashboard.

2. Stel dat nieuwe dashboard als de gebruiker standaard.

3. Verwijder dat Dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Het dashboard is ingesteld in de sitemap

Mogelijk hebt u een standaarddashboard van een organisatie ingesteld door een dashboard te selecteren en ' als standaard instellen ' te kiezen onder ' het systeem aanpassen '. Maar het dashboard dat is gedefinieerd in de sitemapontwerper heeft voorrang op dit dashboard, als de gebruiker er toegang toe heeft.

Als u wilt dat gebruikers het dashboard zien dat u hebt ingesteld als de standaardorganisatie, u:

* Dat Dashboard instellen in de sitemap

* Verwijder de toegang tot het door de sitemap gedefinieerde dashboard voor die gebruikers
