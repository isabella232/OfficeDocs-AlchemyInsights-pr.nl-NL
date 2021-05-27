---
title: Indicatoren werken niet met de Edge-browser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676244"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indicatoren werken niet met de Edge-browser

Nadat u een indicator hebt gemaakt, wordt deze niet geëerd door Edge (Smartscreen). Zie Indicatoren maken [voor IPs en URL's/domeinen voor meer informatie.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Stap 1: Controleer het volgende

- Controleer of de indicator juist is (geen typfouten in IP/URL, juiste actie, de juiste RBAC-groepen).
- Wacht minimaal 2 uur na het maken van de indicator om rekening te houden met eventuele latentie.
- Controleer of het systeem(en) zijn onboarded bij Microsoft Defender voor Eindpunt.
- Controleer of systeem(en) kunnen communiceren met de cloud.
- Controleer of Smartscreen is ingeschakeld en bereikbaar is door naar de [testsite te gaan.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Stap 2: Het mogelijke probleem oplossen

- Zorg ervoor dat de client aan de vereisten voldoet. Zie Indicatoren maken [voor IPs en URL's/domeinen voor meer informatie.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Zorg ervoor dat u de nieuwste versie van de Edge-browser gebruikt. Zie Welke versie van de Microsoft Edge u hebt voor meer informatie over de meest [recente versie.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Start de Edge-browser opnieuw.
- Ga naar de site waarvoor u een indicator hebt ingesteld. Als de site niet wordt weergegeven zoals verwacht, gaat u verder met stap 3. 

## <a name="step-3-collect-data"></a>Stap 3: Gegevens verzamelen

- **MDEClientAnalyzer-diagnostische** gegevens verzamelen. Zie Problemen met [onboarding-machines](issues-with-onboarding-machines.md)bij Microsoft Defender voor Eindpunt voor instructies.
- Zie [Telerik Fiddler](http://www.telerik.com/fiddler)als u vertrouwd bent met het installeren en verzamelen van een Fiddler-trace.
- Als u de voorkeur geeft aan ondersteuning van Microsoft Support, selecteert u het pictogram Ondersteuning hieronder om een ondersteuningscase te openen.
