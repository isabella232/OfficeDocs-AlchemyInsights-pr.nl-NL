---
title: Hulp bij de instelling voor het nachtlampje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404398"
---
# <a name="help-with-the-night-light-display-setting"></a>Hulp bij de instelling voor het nachtlampje

Zie Uw beeldscherm instellen voor [nachttijd in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)voor meer informatie over de weergave-instellingen voor nacht.

Als de opties voor nachtlamp grijs worden weergegeven in Instellingen, controleert u het beeldschermdrijf: 

1. Klik op het zoekvak op de taakbalk en typ **Apparaatbeheer** en selecteer **vervolgens Apparaatbeheer** in de zoekresultaten.
1. Vouw **Beeldschermadapters uit.** 

Helaas is de nachtlampfunctie niet beschikbaar als uw apparaat een DisplayLink-stuurprogramma of een Basic Display-stuurprogramma gebruikt.

De nachtlampfunctie maakt gebruik van recente grafische technologie, dus mogelijk moet u uw beeldschermdrijf bijwerken:  

- Controleer op updates door naar **Instellingen bijwerken starten**  >  **&**  >  **Windows**  >  **Update** controleren  >  **op updates**.  

OF

- Ga naar de ondersteuningswebsite van de hardwarefabrikant om handmatig de nieuwste weergave-stuurprogramma's te downloaden en te installeren.

## <a name="reset-night-light-in-the-registry"></a>Nachtlamp opnieuw instellen in het register

Als het bijwerken van het beeldscherm stuurprogramma niet werkt, moet u mogelijk nachtlamp opnieuw instellen in het register.  

**Let op:** Deze stap voor probleemoplossing wordt alleen aanbevolen voor geavanceerde gebruikers. Er kunnen ernstige problemen optreden als u het register onjuist wijzigt. Voor extra beveiliging maakt u een back-up van het register voordat u het wijzigt, zodat u het kunt herstellen als er problemen optreden.

1. Typ **regedit** in het zoekvak en selecteer **registereditor** in de zoekresultaten.

1. Ga naar de volgende registersleutel: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. De volgende subsleutel exporteren en verwijderen:$$windows.data.bluelightreduction.bluelightreductionstate

1. De volgende subsleutel exporteren en verwijderen:$$windows.data.bluelightreduction.settings

1. Start Windows opnieuw en controleer of de opties voor nachtlamp beschikbaar zijn.


