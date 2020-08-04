---
title: Automatisch opruimen van verouderde apparaten in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554964"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisch opruimen van verouderde apparaten in Intune

Intune stelt de beheerder in staat om een tijdsinterval tussen 90 en 270 dagen te configureren, waarna verouderde apparaten uit de service worden verwijderd. Deze instelling is organisatiebreed en zodra geactiveerd gaat onmiddellijk in werking. Apparaten die gedurende een periode die de instelling overschrijdt, niet in de Intune-server zijn ingecheckt, worden permanent verwijderd.

**Opmerking** Alleen MDM-apparaatobjecten komen in aanmerking voor deze opruimactie. EAS-apparaatobjecten zijn uitgesloten.

Voor aanvullende informatie over wanneer een apparaat in aanmerking komt voor verwijdering op basis van de installatie van het apparaat en de "status":

Instelling: **Apparaten verwijderen na laatste incheckdatum: Ja (enkele waarde (N) in opgegeven dagen)**

- Op basis van de in de instelling geconfigureerde waarde (N) verwijdert de Intune-service het apparaat in de opgegeven dagen nadat het laatste met succes is ingecheckt.

Instelling: **Apparaten verwijderen na laatste incheckdatum: Nee**

- 180 dagen nadat het apparaatcertificaat is verlopen en niet wordt verlengd, wordt het apparaat verwijderd.

**Opmerking** In beide gevallen moet het apparaat met succes worden geregistreerd in Intune. Registratie vindt plaats tijdens het eerste apparaat inchecken met de Intune-service.

Als een apparaat zich met succes inschrijft voor Intune maar niet intune wordt geregistreerd, wordt het apparaat 270 dagen na inschrijving verwijderd. (90 dagen om het apparaat als ingetrokken te markeren en vervolgens nog eens 180 dagen om de record te verwijderen.)

Er bestaat momenteel geen mechanisme in de Intune-console om de vervaldatum van de apparaatcertificering voor een bepaald apparaat vast te stellen.