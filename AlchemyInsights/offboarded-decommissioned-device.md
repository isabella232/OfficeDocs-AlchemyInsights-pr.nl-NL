---
title: Problemen met het verwijderen van een offboarded of buiten bedrijf gesteld apparaat uit de apparaatvoorraad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324439"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemen met het verwijderen van een offboarded of buiten bedrijf gesteld apparaat uit de apparaatvoorraad

Microsoft Defender voor Eindpunt staat momenteel niet toe dat de apparaatrecord van een uitgeschakeld of buiten gebruik gesteld apparaat handmatig wordt verwijderd uit de apparaatvoorraad.

Voor beveiligingsdoeleinden blijft het apparaat tot 180 dagen in de portal staan als een historische record. De apparaatgegevens worden echter verwijderd op basis van de geconfigureerde bewaarperiode.

**Opmerking:** Een uitgeschakeld of buiten bedrijf gesteld apparaat schakelt na zeven dagen automatisch over naar **inactieve** toestand. Bovendien worden apparaten die niet actief zijn in de afgelopen 30 dagen, niet mee verwerkt in de gegevens die uw organisatie weerspiegelen Threat and Vulnerability Management blootstellingsscore of Microsoft Secure Score voor apparaten.
 
Als u bepaalde apparaten nog steeds niet wilt zien in de weergave Apparaatvoorraad, probeert u een apparaatlabel te plaatsen om het buiten bedrijf gesteld apparaat uit de weergave Apparaatvoorraad te filteren.

Zie voor meer informatie:

[Offboard-apparaten van de Microsoft Defender for Endpoint-service](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Blootstellingsscore in Threat and Vulnerability Management](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Ongezonde sensoren in Microsoft Defender voor eindpunt oplossen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Tags effectief gebruiken (deel 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Tags effectief gebruiken (deel 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Tags effectief gebruiken (deel 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




