---
title: Softwarevoorraad ontbreekt of is onjuist
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
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676268"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Softwarevoorraad ontbreekt of is onjuist

De softwarevoorraad in Threat and Vulnerability Management (TVM) is een lijst met bekende software in uw organisatie met de officiële Common Platform Enumerations (CPE).

Softwareproducten zonder een officiële CPE hebben geen beveiligingslekken gepubliceerd. De inventaris bevat ook details, zoals de naam van de leverancier, het aantal zwakke punten, bedreigingen en het aantal blootgestelde apparaten.

Softwarewijzigingen op apparaten worden meestal binnen twee uur doorgevoerd in beveiligingsportalen. Het kan echter soms langer duren. Er is momenteel geen manier om een synchronisatie af te dwingen. dit is een doorlopend doorlopend onderzoek.

Als u een softwarewijziging hebt aangebracht en de wijziging na 5 uur niet nauwkeurig wordt weerspiegeld in TVM, volgt u de volgende stappen:

1. Controleer de sectie software-bewijs om te begrijpen hoe de software is gedetecteerd.
1. Zorg ervoor dat de software wordt ondersteund. Software is mogelijk alleen zichtbaar op apparaatniveau, zelfs als deze momenteel niet wordt ondersteund door Threat and Vulnerability Management. Er zijn echter slechts beperkte gegevens beschikbaar.
1. Zie Onnauwkeurigheid van rapport voor stappen om de onnauwkeurigheid vanuit de portal [te rapporteren.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Opmerking:** Het rapporteren van een onnauwkeurigheid vanuit de MDE-portal is een eenwegkanaal naar engineering. Als het probleem urgent is, opent u een ondersteuningsticket.

Zie Softwarevoorraad - [Threat and Vulnerability Management.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)