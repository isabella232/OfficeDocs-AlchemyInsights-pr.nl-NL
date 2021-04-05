---
title: Schijfruimte vrijmaken in Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505351"
---
# <a name="free-up-drive-space-in-windows-10"></a>Schijfruimte vrijmaken in Windows 10

Hier volgen twee opties voor het vrijmaken van schijfruimte in Windows:

- Schijfruimte vrijmaken in Windows 10.
- Schijfruimte vrijmaken voor Windows 10 updates met extern opslagapparaat.

Als je nog steeds weinig schijfruimte heeft na het gebruiken van Disk Cleanup is het mogelijk dat uw tijdelijke map snel vol geraakt met applicatiebestanden (.appx) die gebruikt worden door Microsoft Store. Los dit probleem op de Store opnieuw in te stellen de cache van de Store te wissen en vervolgens de Windows Update probleemoplosser uit te voeren. Zorg ervoor dat Microsoft Store gesloten is voor je verder gaat met deze stappen.

**Stap 1: Microsoft Store opnieuw instellen**

**Opmerking** Dit verwijdert de app-gegevens op dit apparaat permanent, inclusief je voorkeuren en aanmeldingsgegevens.

1. Selecteer **Start** > **Instellingen** > **Apps** > **Apps en functies**.

1. Vind en selecteer Microsoft Store in de lijst met apps.

1. Selecteer **Geavanceerde opties**.

1. Schuif naar beneden en selecteer **Opnieuw instellen** en vervolgens **Opnieuw instellen bevestigen**.

**Stap 2: de Microsoft Store cache verwijderen**

1. Druk op de Windows-logotoets + R om het dialoogvenster Uitvoeren te openen.

1. Typ in wsreset.exe en selecteer **Ok**.

1. Een lege opdrachtprompt wordt geopend. Na ongeveer 10 seconden wordt het venster gesloten en wordt de Store automatisch geopend.

**Stap 3: Windows update opnieuw instellen**

1. Selecteer **Start** > **Instellingen** > **Updates en beveiliging** > **Probleemzoeker**.

1. Schuif naar beneden en kies **Windows update** uit de lijst en selecteer **Probleemzoeker uitvoeren**.

1. Start de computer opnieuw op en controleer of het probleem zich nog steeds voordoet.

