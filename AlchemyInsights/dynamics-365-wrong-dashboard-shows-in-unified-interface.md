---
title: Dynamics 365-onjuist dashboard wordt weergegeven in de geïntegreerde interface van Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711270"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Onjuiste dashboard wordt weergegeven in de geïntegreerde interface van Dynamics 365

Er zijn verschillende redenen waarom een ander dashboard kan worden weergegeven dan de verwachte versie:

## <a name="the-user-has-set-a-user-default-dashboard"></a>De gebruiker heeft een standaarddashboard voor een gebruiker ingesteld 

Normaalgesproken kunt u aangeven dat het standaarddashboard van een gebruiker is ingesteld als de knop **als standaard instellen** niet wordt weergegeven op de opdrachtbalk van het dashboard. Het standaarddashboard van de gebruiker negeert alle andere standaard dashboards, zelfs als het standaarddashboard van de gebruiker zich niet in de huidige app bevindt.

Gebruik de volgende tijdelijke oplossing om het standaarddashboard uit te heffen.

1. Maak een nieuw, persoonlijk dashboard.

2. Stel dat nieuwe dashboard als standaard instellen.

3. Verwijder het dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Het dashboard is ingesteld op de siteoverzicht

U hebt mogelijk een standaarddashboard voor de organisatie ingesteld door een dashboard te selecteren en ' als standaard instellen ' in te stellen onder ' het systeem aanpassen '. Het dashboard dat in de site van de siteoverzicht is gedefinieerd, heeft voorrang op dit dashboard, als de gebruiker er toegang toe heeft.

Als u wilt dat gebruikers het dashboard kunnen zien dat u hebt ingesteld als de standaardorganisatie, kunt u het volgende doen:

* Dat Dashboard instellen op de siteoverzicht

* De toegang tot het door de site gedefinieerde dashboard voor deze gebruikers verwijderen
