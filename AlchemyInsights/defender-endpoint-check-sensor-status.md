---
title: De status van de Defender Endpoint-sensor controleren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676098"
---
# <a name="defender-endpoint-check-sensor-status"></a>De status van de Defender Endpoint-sensor controleren

De **tegel Apparaten met sensorproblemen** bevindt zich op het dashboard Beveiligingsbewerkingen. Deze tegel bevat informatie over de mogelijkheid van het afzonderlijke apparaat om sensorgegevens te verstrekken en te communiceren met de Defender for Endpoint-service. Het rapport geeft aan hoeveel apparaten aandacht nodig hebben en helpt u problematische apparaten te identificeren en actie te ondernemen om bekende problemen op te lossen.

Twee statusindicatoren op de tegel geven informatie over het aantal apparaten dat niet correct rapporteert aan de service:

- **Verkeerd geconfigureerd** Apparaten die mogelijk gedeeltelijk sensorgegevens rapporteren aan de Defender for Endpoint-service en mogelijk configuratiefouten hebben die moeten worden gecorrigeerd.
- **Inactief** Apparaten die de afgelopen maand meer dan zeven dagen zijn gestopt met rapporteren aan de Defender voor Eindpunt-service.

Als u op een van de groepen klikt, gaat u naar de lijst Apparaten, gefilterd op basis van uw keuzes. In de lijst Apparaten kunt u de lijst met statusstatussen filteren op de volgende status:

- **Actief** Apparaten die actief rapporteren aan de Defender for Endpoint-service.
- **Verkeerd geconfigureerd** Apparaten die mogelijk gedeeltelijk sensorgegevens rapporteren aan de Defender voor Eindpunt-service, maar configuratiefouten hebben die moeten worden gecorrigeerd. Verkeerd geconfigureerde apparaten kunnen een of een combinatie van de volgende problemen hebben:

    - Geen sensorgegevens: apparaten zijn gestopt met het verzenden van sensorgegevens. Beperkte waarschuwingen kunnen worden geactiveerd vanaf het apparaat.
    - Communicatie met een beperking: de mogelijkheid om te communiceren met een apparaat is beperkt. Het verzenden van bestanden voor uitgebreide analyse, het blokkeren van bestanden, het isoleren van apparaten van het netwerk en andere acties waarvoor communicatie met het apparaat is vereist, werkt mogelijk niet.
- **Inactief** Apparaten die niet meer rapporteren aan de Defender voor Eindpunt-service.

U kunt de hele lijst downloaden in CSV-indeling met de functie Exporteren.

Zie De status van [de sensor controleren in Microsoft Defender voor eindpunt voor meer informatie.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Zie Ongezonde sensoren in Microsoft Defender voor eindpunt oplossen voor meer informatie over de oorzaak van inactiviteit of onjuiste configuratie van [een apparaat.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
