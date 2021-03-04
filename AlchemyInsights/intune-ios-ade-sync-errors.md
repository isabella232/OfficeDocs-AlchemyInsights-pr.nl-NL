---
title: Apple Automatische apparaatinschrijvingssynchronisatiefouten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448917"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple Automatische apparaatinschrijvingssynchronisatiefouten

'We hebben vastgesteld dat u een of meer ADE/DEP-tokens hebt met een fouttoestand. Totdat de fouttoestand voor elk beïnvloed token is opgelost, werkt de ADE-functionaliteit niet meer zoals verwacht.'

Deze fout kan zich op een aantal manieren voor doen, waaronder:

1. Apparaten worden mogelijk niet gesynchroniseerd tussen ABM/ASM en Intune
2. Inschrijvingsprofieltoewijzingen zijn mogelijk mislukt
3. ADE-inschrijving kan mogelijk niet worden voltooid

Controleer of de synchronisatiefout is gerapporteerd in de Intune-console onder **Apparaten > Apparaten > Apple-inschrijving**> programmatokens voor registratie.

Een van de meest voorkomende oorzaken van een synchronisatiefout is het verlopen van het huidige token. In veel gevallen wordt het probleem verholpen door het verlengen van het betreffende token.

Als een of meer van uw tokens zijn verlopen, kunt u deze in de volgende documentatie verlengen:

[Een token voor automatische inschrijving van apparaten verlengen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Bovendien kunt u de volgende documentatie bekijken om mogelijke herstelmogelijkheden voor andere fouten te bekijken die synchronisatiefouten in token veroorzaken:

[ABM/ASM-synchronisatiefouten voor iOS/iPadOS en macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-synchronisatiefouten voor iOS/iPadOS en macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
