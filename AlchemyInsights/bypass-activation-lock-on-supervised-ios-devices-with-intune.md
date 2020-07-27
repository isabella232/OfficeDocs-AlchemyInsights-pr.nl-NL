---
title: Activeringsvergrendeling omzeilen op iOS-apparaten onder toezicht met Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423489"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Activeringsvergrendeling omzeilen op iOS-apparaten onder toezicht met Intune

De mogelijkheid om het activeringsslot op iOS-apparaten te omzeilen, maakt het gemakkelijker om te herstellen van het scenario waarin een gebruiker activeringsvergrendeling op een bedrijfsapparaat inschakelt en verlaat het bedrijf.

Vereisten voor het omzeilen van een activeringsslot zijn:

- Een apparaat is dat is "gecontroleerd."
- Het activeringsslot is ingeschakeld met het beperkingsbeleid van iOS-apparaten in Intune.

Bovendien moet u bij het omzeilen van een activeringsslot:

- Fysiek bezit het apparaat wordt gewist.
- Kopieer de code voordat u het wissen uitgave.

**Let op:** De veegcode is niet gevoelig voor de zaak, dus de "-" tekens zijn niet vereist.

Zie [Bypass-activeringsvergrendeling op iOS-apparaten met Intune voor](https://docs.microsoft.com/intune/device-activation-lock-bypass)meer informatie.

**Veelgestelde vragen**

V: **Ik heb een actie op afstand uitgevaardigd om bedrijfsgegevens van een apparaat te verwijderen en nu zit deze vast in een in behandeling zijnde status.**

A: Om een actie op afstand succesvol te voltooien, moet het beoogde apparaat online en gezond zijn. In de volgende situaties blijft de actie op afstand 30 dagen in behandeling of totdat het apparaat de opdracht erkent wanneer het apparaat:

- Heeft geen connectiviteit.
- Verliest zijn managementstatus bij Intune.

Als u denkt dat een apparaat niet meer incheckt en bedrijfsgegevens niet verwijdert, selecteert u Verwijderen. Als u de apparaatrecord verwijdert, wordt de apparaatrecord verwijderd, zodat deze niet meer wordt weergegeven in de Intune-lijst met apparaten. Als het apparaat weer actief wordt, moet de gebruiker het apparaat opnieuw inschrijven.

V: **Waarom zijn bepaalde acties op afstand niet beschikbaar voor mij om te gebruiken?**

A: Niet alle platforms ondersteunen alle acties op afstand. De volgende acties op afstand zijn platformspecifiek.

- Activeringsvergrendeling omzeilen (alleen iOS)
- Nieuwe start (alleen Windows)
- Verloren modus (alleen iOS)
- Apparaat zoeken (alleen iOS)
- Opnieuw opstarten (alleen Windows)

Zie Acties voor beschikbare [apparaten](https://docs.microsoft.com/intune/device-management#available-device-actions)voor meer informatie over elke actie.