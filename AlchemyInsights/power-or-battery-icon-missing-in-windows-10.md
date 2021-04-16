---
title: Stroom- of batterijpictogram ontbreekt in Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790543"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Stroom- of batterijpictogram ontbreekt in Windows 10

Als uw Windows 10-apparaat een batterij heeft (bijv. een laptop of tablet, of een pc die via USB is aangesloten op een UPS), wordt normaal gesproken een stroom-/batterijpictogram in de taakbalk naast de klok weergegeven, bijvoorbeeld:

![Batterijpictogram](media/battery-icon.png)

Als u dit pictogram niet ziet, is het mogelijk verborgen:

1. Ga naar **[Instellingen > Persoonlijke instellingen > Taakbalk](ms-settings:taskbar?activationSource=GetHelp)**.

2. Klik in het systeemvenster op **Selecteer welke pictogrammen op de taakbalk worden weergegeven**.

3. Zoek vervolgens het **Power**-item in de lijst en zet de instelling op **Aan**.

    ![Power-pictogram weergeven op de taakbalk](media/power-icon-on.png)

**Problemen oplossen**

Als u de bovenstaande instructies hebt gevolgd en de schakelknop **Power** grijs wordt weergegeven of niet zichtbaar is, typt u **Device Manager** in het zoekvak op de taakbalk en selecteert u **Device Manager** in de lijst met resultaten. Klik onder **Batterijen** met de rechtermuisknop op de batterij van uw apparaat, klik op **Uitschakelen** en klik op **Ja**. Wacht een paar seconden, klik met de rechtermuisknop op de batterij en klik op **Inschakelen**. Start het apparaat vervolgens opnieuw op.

Als u de bovenstaande instructies hebt gevolgd, maar het batterijpictogram niet wordt weergegeven op de taakbalk, typt u **taakbeheer** in het zoekvak op de taakbalk en klikt u vervolgens op **Taakbeheer** in de lijst met resultaten. Klik op het tabblad **Processen**, onder **Naam**, met de rechtermuisknop op **Explorer** en klik vervolgens op **Opnieuw opstarten**.
