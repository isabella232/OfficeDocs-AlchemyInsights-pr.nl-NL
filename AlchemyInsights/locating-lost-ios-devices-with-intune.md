---
title: Verloren iOS-apparaten lokaliseren met Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439143"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Verloren iOS-apparaten lokaliseren met Intune

Als u de verloren modus op een iOS-apparaat inschakelt, kan een beheerder een bericht en telefoonnummer op het vergrendelingsscherm weergeven.

Nadat de verloren modus is ingeschakeld, kan de beheerder de actie Apparaat lokaliseren gebruiken om de fysieke locatie van het apparaat te identificeren.

De actie Apparaat zoeken in Intune werkt met iOS-apparaten om de locatie van een specifiek apparaat op een kaart weer te geven.

Voor het gebruik van deze actie moet het iOS-apparaat zich in:

- Bewaakte modus
- Verloren modus

Zie [Verloren modus inschakelen op iOS/iPadOS-apparaten met Intune](https://docs.microsoft.com/intune/device-lost-mode) en Verloren verloren [iOS/iPadOS-apparaten lokaliseren met Intune](https://docs.microsoft.com/intune/device-locate)voor meer informatie.

**Veelgestelde vragen**

V: Ik heb een actie op afstand uitgevaardigd om bedrijfsgegevens van een apparaat te verwijderen en nu zit deze vast in een in behandeling zijnde status.

A: Om een actie op afstand succesvol te voltooien, moet het beoogde apparaat online en gezond zijn. In de volgende situaties blijft de actie op afstand 30 dagen in behandeling of totdat het apparaat de opdracht erkent:

- Wanneer het apparaat geen verbinding heeft
- Wanneer het apparaat zijn beheerstatus verliest met Intune

Als u denkt dat een apparaat niet meer incheckt en als het bedrijfsgegevens niet kan verwijderen, selecteert u Verwijderen. Als u de apparaatrecord verwijdert, wordt de apparaatrecord verwijderd, zodat deze niet meer wordt weergegeven in de Intune-lijst met apparaten. Als het apparaat weer actief wordt, moet de gebruiker het opnieuw inschrijven.

V: Waarom zijn bepaalde acties op afstand niet beschikbaar voor mij om te gebruiken?

A: Niet alle platforms ondersteunen alle acties op afstand. De volgende externe acties zijn platformspecifiek, dus ze zijn alleen beschikbaar voor de genoemde platforms.

- Activeringsvergrendeling omzeilen (alleen iOS)
- Nieuwe start (alleen Windows)
- Verloren modus (alleen iOS)
- Apparaat zoeken (alleen iOS)
- Opnieuw opstarten (alleen Windows)

Zie Acties voor beschikbare [apparaten](https://docs.microsoft.com/intune/device-management#available-device-actions)voor meer informatie over elke actie.