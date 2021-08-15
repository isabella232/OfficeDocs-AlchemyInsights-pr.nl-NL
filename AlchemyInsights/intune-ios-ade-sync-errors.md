---
title: Synchronisatiefouten voor automatische registratie van Apple-apparaat
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013743"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisatiefouten voor automatische registratie van Apple-apparaat

"We hebben vastgesteld dat u een of meer ADE/DEP-tokens hebt die een fouttoestand hebben. Totdat de fouttoestand is opgelost voor elk van de betrokken tokens, werkt de ADE-functionaliteit niet zoals verwacht.'

Deze fout kan zich op een aantal manieren manifesteert, waaronder:

1. Apparaten worden mogelijk niet gesynchroniseerd van ABM/ASM naar Intune
2. Inschrijvingsprofieltoewijzingen kunnen mislukken
3. Apparaten kunnen ADE-inschrijving mogelijk niet voltooien

Controleer of de synchronisatiefout is gerapporteerd in de Intune-console onder Apparaten > Apparaten > Apple-registratie-> **Enrollment program tokens**.

Een van de meest voorkomende oorzaken van synchronisatiefouten is het verlopen van het huidige token. In veel gevallen wordt het probleem opgelost door het betreffende token te verlengen.

Als een of meer van uw tokens zijn verlopen, bekijkt u de volgende documentatie om ze zo nodig te verlengen:

[Een token voor het automatisch registreren van apparaten verlengen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Daarnaast kunt u de volgende documentatie bekijken om mogelijke herstelmogelijkheden te zien voor andere fouten die tokensynchronisatiefouten veroorzaken:

[ABM/ASM-synchronisatiefouten voor iOS/iPadOS en macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-synchronisatiefouten voor iOS/iPadOS en macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
