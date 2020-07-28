---
title: Inventaris van intune-apparaten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439159"
---
# <a name="intune-device-inventory"></a>Inventaris van intune-apparaten

Het apparaat van de apparaten geeft de beheerder inzicht in apparaten die onder beheer zijn in Intune per apparaat. De getoonde informatie omvat: Hardware, Gedetecteerde toepassingen, status apparaatnaleving en status apparaatconfiguratie.

Voorraadgegevens voor hardware en gedetecteerde toepassingen worden verzameld op een cyclus van zeven dagen. De toepassingen en specifieke elementen van de gerapporteerde hardware verschillen afhankelijk van het besturingssysteem van het apparaat en of het apparaat persoonlijk of eigendom van het bedrijf is.

[Zie Apparaatgegevens in Intune voor](https://docs.microsoft.com/intune/device-inventory)meer informatie.

**Veelgestelde vragen**

V: Ik ontvang geen volledige voorraadlijst van toepassingen die aanwezig zijn op Intune-ingeschreven Windows-apparaten. Waarom niet?

A: Op dit moment worden alleen moderne apps weergegeven voor Windows 10-pc's die zijn geïdentificeerd als bedrijfsapparaten. Intune verzamelt geen informatie over Win32-apps die op deze apparaten zijn geïnstalleerd.

V: Waarom worden telefoonnummers niet verzameld van alle apparaten?

A: Telefoons die zijn gecategoriseerd als bedrijfsapparaten in Intune, worden niet geïdentificeerd met hun volledige telefoonnummer wanneer u bijvoorbeeld een inventarisrapport voor mobiele apparaten uitvoert. Telefoonnummers voor bring-you-own-device worden altijd gedeeltelijk gemaskeerd met sterretjes (****), en tonen alleen de laatste vier cijfers.