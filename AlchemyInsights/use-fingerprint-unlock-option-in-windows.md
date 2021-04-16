---
title: De optie Vingerafdruk ontgrendelen gebruiken in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796672"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>De optie Vingerafdruk ontgrendelen gebruiken in Windows 10

**Windows Hello Fingerprint inschakelen**

Als u Windows 10 wilt ontgrendelen met uw vingerafdruk, moet u Windows Hello Fingerprint instellen door ten minste één vinger toe te voegen (zodat Windows leert herkennen). 

1. Ga naar **Instellingen > Accounts > aanmeldingsopties** (of klik [hier).](ms-settings:signinoptions?activationSource=GetHelp) Beschikbare aanmeldingsopties worden weergegeven. Bijvoorbeeld:

    ![Aanmeldingsopties.](media/sign-in-options.png)

2. Klik of tik op **Windows Hello Fingerprint** en klik vervolgens op **Instellen.** Klik in het windows Hello-installatievenster op **Aan de slag.** De vingerafdruk sensor wordt geactiveerd en u wordt gevraagd uw vinger op de sensor te plaatsen:

   ![Vingerafdruk sensor.](media/fingerprint-sensor.png)

3. Volg de instructies, waarmee u wordt gevraagd uw vinger herhaaldelijk te scannen. Wanneer dit is voltooid, kunt u andere vingers toevoegen die u mogelijk wilt gebruiken voor aanmelding. De volgende keer dat u zich bij Windows 10 aan melden, hebt u de mogelijkheid om uw vingerafdruk te gebruiken om dit te doen.

**Windows Hello Fingerprint niet beschikbaar als aanmeldingsoptie**

Als Windows Hello Fingerprint niet wordt weergegeven als een optie **in** aanmeldingsopties, betekent dit dat Windows niet op de hoogte is van een vingerafdruklezer/scanner die aan uw pc is gekoppeld of dat een systeembeleid het gebruik ervan verhindert (als uw pc bijvoorbeeld wordt beheerd door uw werkplek). Problemen oplossen: 

1. Selecteer de **knop Start** op de taakbalk en zoek **naar Apparaatbeheer.**

2. Klik of tik om **Apparaatbeheer te openen.**

3. Vouw in Apparaatbeheer biometrische apparaten uit door op de punthaak te klikken.

   ![Biometrische apparaten.](media/biometric-devices.png)

4. Uw vingerafdrukscanner moet worden weergegeven als een biometrisch apparaat, zoals de Synaptics WBDI-scanner:

   ![Biometrische apparaten.](media/biometric-devices-expanded.png)

5. Als uw vingerafdrukscanner niet wordt weergegeven en de scanner is geïntegreerd in uw pc, gaat u naar de website van de fabrikant van de pc. Zoek in de sectie technische ondersteuning voor uw pc-model naar een Windows 10-stuurprogramma voor een scanner die u kunt installeren.

6. Als de scanner is gescheiden van de pc (gekoppeld via USB), gaat u naar de website van de fabrikant van de scanner om de stuurprogrammasoftware van Windows 10 te zoeken en te installeren voor het scannermodel dat u hebt.
