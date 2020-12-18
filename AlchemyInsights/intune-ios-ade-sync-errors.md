---
title: Synchronisatiefouten met Apple-apparaten voor automatisch registreren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714738"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisatiefouten met Apple-apparaten voor automatisch registreren

' We hebben vastgesteld dat er een of meer ADE-of DEP-tokens zijn met een foutstatus. Wanneer de foutstatus voor elk kwetsbaar token is opgelost, werkt de ADE-functionaliteit niet voor hetzelfde.

Deze fout kan op verschillende manieren worden weergegeven, zoals:

1. Apparaten worden mogelijk niet gesynchroniseerd van ABM/ASM naar intune
2. Toewijzing van registratie profielen is mogelijk mislukt
3. Mogelijk is de herregistratie van de hardware niet voltooid

Controleer of de synchronisatiefout is gerapporteerd in de intune-console onder **apparaten > schrijf apparatuur > Apple enrollment > tokens voor het registratieprogramma** en Raadpleeg de volgende documentatie voor een potentiële herstelactie:

[Synchronisatiefouten in ABM/ASM voor iOS/iPadOS en macOS-registratie tokens voor automatisch apparaat](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
