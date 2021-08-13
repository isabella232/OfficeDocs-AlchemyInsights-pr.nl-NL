---
title: Gegevens verwijderen en apparaten wissen uit Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922205"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Gegevens verwijderen en apparaten wissen uit Intune

Met de acties apparaat buiten gebruik stellen en apparaat wissen kunnen bedrijfsgegevens die beheerd worden door Intune verwijderd worden of de fabrieksinstellingen opnieuw ingesteld worden.

1. Meld je aan in Microsoft 365-apparaatbeheer en ga naar **Apparaten** > **Alle apparaten**.
2. Selecteer het apparaat dat je wilt wissen.
3. Selecteer het type wissen van op afstand dat je wilt uitvoeren. Buiten gebruik stellen verwijdert enkel informatie van de organisatie. Volledig wissen herstelt de fabrieksinstellingen op het apparaat. 
4. Selecteer **Ja** om te bevestigen. Totdat wissen voltooid is wordt de status van het apparaat als *buiten gebruik stellen in behandeling* weergegeven.
    Nadat de actie voltooid is wordt het mobiele apparaat niet meer in de lijst van beheerde apparaten weergegeven.

> [!NOTE]
> Bedrijfsgegevens kunnen niet verwijderd worden uit apparaten die aan Azure AD toegevoegd zijn. 

Voor een volledig overzicht van de gevolgen van de acties buiten gebruik stellen en wissen, inclusief wat behouden wordt en wat verwijderd wordt, zie de volgende documentatie:

- [Apparaten verwijderen met wissen, buiten gebruik stellen of het apparaat manueel uitschrijven](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Hoe enkel bedrijfsgegevens wissen uit Intune-beheerde apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Alle gegevens wissen uit een macOS-apparaat](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).