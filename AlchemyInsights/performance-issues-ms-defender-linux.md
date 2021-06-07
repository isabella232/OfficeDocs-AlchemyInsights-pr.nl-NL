---
title: Prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793760"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux

In dit artikel wordt u begeleid bij de stappen voor het identificeren van prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux.

Het is belangrijk om eerst te controleren of het probleem dat u ondervindt, is opgelost met de [nieuwste versie.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Zie Prestatieproblemen oplossen voor Microsoft Defender voor Eindpunt op Linux om uw onderzoek [te starten.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Uitsluitingen

Uitsluitingen kunnen helpen om prestatieproblemen te beperken. Controleer uw uitsluitingen voordat u begint, zodat eventuele extra risico's bekend en gedocumenteerd zijn.

Zie Uitsluitingen [configureren en valideren](/microsoft-365/security/defender-endpoint/linux-exclusions)voor Microsoft Defender voor Eindpunt op Linux voor meer informatie.

Als u meerdere bestanden & mappen die u wilt uitsluiten en ze allemaal op hetzelfde mountpoint staan, is het mogelijk gemakkelijker om het mountpoint uit te sluiten. Vanaf release 101.22.80 van februari kunt u een volledig bevestigingspunt uitsluiten.

Als bijvoorbeeld /mnt/back-up een mountpoint is, kunt u /mnt/back-up toevoegen aan de lijst met uitsluiten door deze opdracht uit te voeren:

`$ mdatp exclusion folder add –path /mnt/backup`

**Opmerking:** Het toevoegen van uitsluitingen verhoogt het risico dat malware niet wordt gedetecteerd en moet zorgvuldig worden verwerkt en geïmplementeerd.

## <a name="need-help"></a>Hulp nodig?

Als u u op de meest efficiënte manier wilt helpen, verzamelt u de diagnostische gegevens voordat u een ondersteuningscase opent.
