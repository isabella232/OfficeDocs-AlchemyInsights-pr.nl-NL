---
title: Schijfruimte vrij maken in Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035666"
---
# <a name="free-up-drive-space-in-windows-10"></a>Schijfruimte vrij maken in Windows 10

Hier zijn twee opties om schijfruimte vrij te maken in Windows:

- Schijfruimte vrij maken in Windows 10.
- Ruimte vrij maken voor Windows 10-updates met een extern opslagapparaat.

Als u na het gebruik van Schijfopruiming nog steeds weinig schijfruimte hebt, is het mogelijk dat de map Temp snel wordt gevuld met toepassingsbestanden (.appx) die door Microsoft Store worden gebruikt. U kunt dit probleem oplossen door de Store opnieuw in te stellen, de Store-cache te wissen en vervolgens de probleemoplosser voor Windows Update uit te voeren. Zorg ervoor dat de Microsoft Store is gesloten voordat u verder gaat met deze stappen.

**Stap 1: Microsoft Store opnieuw instellen**

**Opmerking** Hiermee worden de app-gegevens op het apparaat definitief verwijderd, inclusief uw voorkeuren en aanmeldingsgegevens.

1. Selecteer **Instellingen instellingen**  >  **apps** starten  >  **Apps**&  >  **functies**.

1. Zoek en selecteer Microsoft Store in de lijst met apps.

1. Selecteer **Geavanceerde opties.**

1. Schuif omlaag en selecteer **Opnieuw instellen** en bevestig **opnieuw instellen.**

**Stap 2: De Microsoft Store-cache wissen**

1. Druk op de Windows-logotoets + R om het dialoogvenster Uitvoeren te openen.

1. Typ wsreset.exe en selecteer **OK.**

1. Er wordt een leeg venster met opdrachtprompt geopend. Na ongeveer 10 seconden wordt het venster gesloten en wordt de Store automatisch geopend.

**Stap 3: Windows Update opnieuw instellen**

1. Selecteer **Instellingen bijwerken**  >  **starten** om &  >  **beveiligingsproblemen op te**  >  **lossen.**

1. Schuif omlaag en selecteer **Windows Update** in de lijst en selecteer **De probleemoplosser uitvoeren.**

1. Start uw computer opnieuw op en controleer of u het probleem nog steeds ondervindt.

