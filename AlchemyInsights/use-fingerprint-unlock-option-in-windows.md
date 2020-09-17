---
title: De optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795239"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>De optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10

**Windows hello-vingerafdruk inschakelen**

Als u Windows 10 wilt ontgrendelen met behulp van uw vingerafdruk, moet u de vingerafdruk van Windows hello instellen door het toevoegen (laat Windows leren herkend) ten minste één vinger. 

1. Ga naar **instellingen > Accounts > aanmeldingsopties** (of Klik [hier](ms-settings:signinoptions?activationSource=GetHelp).) De beschikbare aanmeldingsopties worden weergegeven. Bijvoorbeeld:

    ![Aanmeldingsopties.](media/sign-in-options.png)

2. Klik of tik op de **vingerafdruk van Windows hello**en klik vervolgens op **instellen**. Klik in het venster Windows hello instellen op **aan de slag**. De vingerafdruksensor wordt geactiveerd, waarna u wordt gevraagd uw vinger op de sensor te plaatsen:

   ![Vingerafdruksensor.](media/fingerprint-sensor.png)

3. Volg de instructies om u te vragen uw vinger herhaaldelijk te scannen. Wanneer dit is gebeurd, kunt u nog andere vingers toevoegen die u mogelijk wilt gebruiken om u aan te melden. De volgende keer dat u zich aanmeldt bij Windows 10, kunt u uw vingerafdruk ook gebruiken.

**De vingerafdruk van Windows hello is niet beschikbaar als aanmeldingsoptie**

Als u de vingerafdruk van Windows Hello niet als optie **ziet, betekent**dit dat Windows niet op de hoogte is van een vingerafdruklezer/scanner die is aangesloten op uw PC, of dat een systeembeleid het gebruik ervan verhindert (als uw pc bijvoorbeeld wordt beheerd door uw werk). Problemen oplossen: 

1. Selecteer de knop **Start** op de taakbalk en zoek **Apparaatbeheer**.

2. Klik of tik om **Apparaatbeheer**te openen.

3. Vouw in Apparaatbeheer de biometrische apparaten uit door te klikken op de dubbele punthaak.

   ![Biometrische apparaten.](media/biometric-devices.png)

4. De vingerafdrukscanner moet als een biometrisch apparaat worden weergegeven, zoals de Synaptics WBDI-scanner:

   ![Biometrische apparaten.](media/biometric-devices-expanded.png)

5. Ga naar de website van de fabrikant van de PC als de vingerafdrukscanner niet wordt weergegeven en de scanner is geïntegreerd in uw PC. Zoek in de sectie technische ondersteuning voor uw PC-model naar een Windows 10-stuurprogramma voor een scanner die u kunt installeren.

6. Als de scanner losstaat van de PC (aangesloten via USB), gaat u naar de website van de scannerfabrikant om Windows 10-stuurprogrammasoftware te zoeken en te installeren voor uw scannermodel.
