---
title: Opstartinstellingen in Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828147"
---
# <a name="startup-settings-in-windows-10"></a>Opstartinstellingen in Windows 10

**Wijzigen welke apps automatisch worden uitgevoerd bij het opstarten**

1. Ga naar [Instellingen > Apps > Opstarten.](ms-settings:startupapps?activationSource=GetHelp)

2. Zorg ervoor dat een app die u wilt uitvoeren bij het opstarten is **ingeschakeld.**

**Een app toevoegen die automatisch moet worden uitgevoerd bij het opstarten**

1. Klik of tik op **Start** en zoek de app die u wilt uitvoeren bij het opstarten.

2. Klik met de rechtermuisknop op de app, klik **op Meer** en klik vervolgens **op Bestandslocatie openen.** Hiermee wordt de locatie geopend waar de snelkoppeling naar de app wordt opgeslagen. Als er geen optie is voor Bestandslocatie openen, betekent dit dat de app niet kan worden uitgevoerd bij het opstarten.

3. Als de bestandslocatie is geopend, drukt u op **de Windows-logotoets + R**, typt u **shell:startup** en klikt u vervolgens op **OK.** Hiermee wordt de map Opstarten geopend.

4. Kopieer en plak de snelkoppeling naar de app van de bestandslocatie naar de map Opstarten.

**Geavanceerde opstartopties (inclusief veilige modus, UEFI-instellingen en opstarten vanaf een ander apparaat)**

1. Sla uw werk op en sluit alle geopende documenten, omdat uw pc met deze stappen opnieuw wordt gestart.

2. Ga naar [Instellingen > & beveiligingsherstel > bijwerken.](ms-settings:recovery?activationSource=GetHelp)

3. Klik **onder Geavanceerd opstarten** op Nu opnieuw **starten.** 

4. Nadat uw pc opnieuw is gestart naar het scherm Kies een optie:

    - Als u wilt opstarten vanaf een apparaat zoals een USB-station, klikt u **op Een apparaat gebruiken.**

    - Als u de UEFI-instellingen (ook wel BIOS-instelling genoemd) wilt invoeren, klikt u op Problemen oplossen > Geavanceerde opties > **UEFI Firmware-instellingen.** 

    - Als u de veilige modus wilt invoeren of geavanceerde opstartinstellingen wilt wijzigen, klikt u op Problemen oplossen > Geavanceerde opties > **Opstartinstellingen** en klikt u vervolgens op **Opnieuw starten.** Mogelijk wordt u gevraagd uw [BitLocker-herstelsleutel in te voeren.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Nadat uw pc opnieuw is gestart, klikt u op de instelling voor opstarten die u wilt gebruiken.