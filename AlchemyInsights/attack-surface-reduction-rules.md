---
title: Regels voor het verminderen van kwetsbaarheid voor aanvallen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676127"
---
# <a name="attack-surface-reduction-rules"></a>Regels voor het verminderen van kwetsbaarheid voor aanvallen

Het uitsluiten van bestanden of mappen kan de beveiliging die wordt geboden door regels voor het beperken van het oppervlak van de aanval, aanzienlijk beperken. Bestanden die door een regel zijn geblokkeerd, mogen worden uitgevoerd en er wordt geen rapport of gebeurtenis opgenomen. Een uitsluiting is van toepassing op alle regels die uitsluitingen toestaan.

Asr-uitsluitingen gebruiken dezelfde syntaxis als Microsoft Defender Antivirus uitsluitingen. Zie Uitsluitingen [configureren en valideren voor](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)Microsoft Defender Antivirus scans voor meer informatie. Als u problemen wilt voorkomen, bekijkt u [Veelvoorkomende fouten om te voorkomen bij het definiëren van uitsluitingen.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Niet alle ASR-regels ondersteunen uitsluitingen. Als u wilt valideren of uw regel uitsluitingen ondersteunt, bekijkt u de tabel [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regels voor het verminderen van kwetsbaarheid voor aanvallen

De surface van uw organisatie-aanval bevat alle locaties waar een aanvaller organisatieapparaten of netwerken kan compromitteerden. Als u uw aanvalsoppervlak verkleint, moet u de organisatieapparaten en het netwerk beschermen, waardoor aanvallers minder manieren hebben om aanvallen uit te voeren. Het configureren van regels voor het verlagen van de Surface-aanval in Microsoft Defender voor Eindpunt kan u helpen.

Zie voor meer informatie:

- [ASR-regel GUID aan een naam geven](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- VEREISTEN VOOR ASR-regels:
    - [Windows 10 Pro, versie 1709 of hoger](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versie 1709 of hoger](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versie 1803 (halfjaarlijks kanaal) of hoger](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>De juiste uitsluiting identificeren die moet worden toegepast

1. Zoek naar eventID 1121 of 1122 in het Microsoft-Windows-Windows Defender/Operational log.

1. Evalueer het blokscenario en de context en bevestig dat dit scenario moet worden geblokkeerd.

1. Lees de waarde Pad in de gebeurtenisdetails, de waarde die de uitsluiting definieert.
    - Maak de uitsluiting zo strikt mogelijk.
    - Pas indien nodig een jokerteken toe (vervang bijvoorbeeld de variabele Gebruiker).

1. Pas de uitsluiting toe op basis van uw implementatiebehoeften. Zie Attack [Surface Reduction Rules aanpassen voor meer informatie.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Uitsluiting wordt niet nagekomen

1. Bepaal of de regel uitsluitingen ondersteunt. Zie Surface [Reduction Rules attack (Surface Reduction Rules) voor meer informatie.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Controleer de toegepaste uitsluitingen en controleer met de gebeurtenisgegevens op typefouten of onjuist geïnterpreteerde jokertekens. Zie Ondersteunde [uitsluitingstypen voor meer informatie](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. als de invloed van de regel te hoog is, kunt u overwegen de regel (terug) te verplaatsen naar de auditmodus om verdere validatie uit te voeren. Zie Testen hoe Microsoft Defender voor eindpuntfuncties werken [in de auditmodus](/microsoft-365/security/defender-endpoint/audit-windows-defender)voor meer informatie.

1. Verzamel ondersteuningsgegevens om een ondersteuningscase te openen met behulp van deze opdracht:
    
   ** MDEClientAnalyzer.cmd -v**

    Zie Problemen met [onboarding-machines](issues-with-onboarding-machines.md)bij Microsoft Defender voor eindpunten voor meer informatie.
