---
title: Gegevens verwijderen en apparaten wissen van Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439156"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Gegevens verwijderen en apparaten wissen van Intune

De acties Device Retire en Device Wipe kunnen worden gebruikt om bedrijfsgegevens te verwijderen die door Intune worden beheerd of om een fabrieksreset uit te voeren en het apparaat terug te sturen naar de standaardinstellingen.

1. Meld u aan bij Microsoft 365 Device Management en ga naar **Apparaten**  >  **alle apparaten**.
2. Selecteer het apparaat dat u wilt wissen.
3. Selecteer het type externe veeg die u wilt maken. Met pensioen gaat alleen organisatorische informatie, terwijl volledige doekjes het apparaat herstellen naar de fabrieksinstellingen.
4. Selecteer **Ja** om te bevestigen. Totdat het wissen is voltooid, wordt de actiestatus Apparaat weergegeven als In behandeling met pensioen.</br>
    Nadat de actie is voltooid, ziet u het mobiele apparaat niet meer in de lijst met beheerde apparaten.

**Opmerking** Bedrijfsgegevens kunnen niet worden verwijderd van apparaten die zijn aangesloten bij Azure AD.

Zie Apparaten verwijderen met behulp van [het apparaat wissen, met pensioen en handmatig uitrollen van het apparaat voor](https://docs.microsoft.com/intune/devices-wipe)meer informatie over het effect van de acties Met pensioen gaan en wissen, inclusief wat wordt bewaard en wat wordt verwijderd.

Zie [Alle gegevens van een macOS-apparaat wissen als](https://docs.microsoft.com/intune/device-erase)u alle gegevens van een macOS-apparaat wilt wissen.