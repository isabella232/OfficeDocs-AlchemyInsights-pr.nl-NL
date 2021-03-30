---
title: EndPoint Manager - Basislijnen voor beveiliging
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420775"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Basislijnen voor beveiliging

Beveiligingslijnlijnen zijn vooraf geconfigureerde groepen Windows-instellingen die u helpen bij het toepassen van de beveiligingsinstellingen die worden aanbevolen door de relevante beveiligingsteams. Deze basislijnen kunnen worden aangepast om alleen de gewenste instellingen en waarden te leveren. Zie Beveiligingslijnlijnen gebruiken om [Windows 10-apparaten in Intune te configureren voor meer informatie over beveiligingslijnlijnen.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Er zijn momenteel basislijnen voor deze producten:

- Windows MDM-beveiligingsinstellingen
- Microsoft Defender voor EndPoint-beveiliging
- Microsoft Edge

Elk van de basislijnen wordt regelmatig bijgewerkt en uitgebracht in incrementele versies. Met elke versie worden instellingen uit de vorige versie toegevoegd en of verwijderd om ervoor te zorgen dat de basislijn voldoet aan de huidige richtlijnen. Met de console Beveiligingslijnlijnen in Endpoint Security kunnen verschillende versies worden vergeleken door de wijzigingen van versie naar versie zichtbaar te maken.

Zie Beveiligingslijnprofielen beheren [in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)voor informatie over het zo effectief mogelijk wijzigen van welke versie van basislijn wordt geïmplementeerd.

Nadat u een beveiligingslijn hebt geïmplementeerd, kunt u de status van de implementatie controleren en de instellingen per apparaat controleren.

**Opmerking:** Het kan maximaal 24 uur duren voordat de rapportagegegevens voor basislijnen worden weergegeven vanaf de eerste implementatie naar een apparaat en tot 6 uur voor verdere updates. 

De meest voorkomende oorzaak van het niet toepassen van een basislijninstelling is omdat dezelfde instelling wordt gebruikt in een ander profiel. Dit scenario kan worden onderzocht voor een specifiek apparaat door dat apparaat te selecteren in het knooppunt Apparaatstatus van het beveiligingslijnprofiel. Zie Conflicten voor beveiligingslijnlijnen oplossen voor meer [informatie.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)