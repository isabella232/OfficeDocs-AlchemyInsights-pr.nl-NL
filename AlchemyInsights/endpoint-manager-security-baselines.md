---
title: EndPoint Manager - beveiligingsbasislijnen
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978156"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - beveiligingsbasislijnen

Beveiligingsbasislijnen zijn vooraf geconfigureerde groepen Windows-instellingen die u helpen bij het toepassen van de beveiligingsinstellingen die door de relevante beveiligingsteams worden aanbevolen. U kunt deze basislijnen aanpassen om alleen de instellingen en waarden te kunnen leveren. Voor meer informatie over beveiligingsbasislijnen, zie [Beveiligingsbasislijnen gebruiken om Windows 10-apparaten te configureren in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Er zijn momenteel basislijnen voor deze producten:

- Windows MDM-beveiligingsinstellingen
- Microsoft Defender voor eindpuntbeveiliging
- Microsoft Edge

Alle basislijnen wordt periodiek bijgewerkt en uitgebracht in incrementele versies. In elke versie worden instellingen toegevoegd en verwijderd uit de vorige versie om ervoor te zorgen dat de basislijn voldoet aan de huidige richtlijnen. Met de console voor beveiligingsbasislijnen in Eindpuntbeveiliging, kunnen verschillende versies worden vergeleken door de wijzigingen van versie naar versie zichtbaar te maken.

Voor instructies om zo effectief mogelijk te wijzigen welke basislijnversie is geïmplementeerd, zie [Profielen voor beveiligingsbasislijn beheren in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Nadat u een basislijn voor beveiliging hebt geïmplementeerd, kunt u de status van de implementatie controleren en de instellingen per apparaat controleren.

**Opmerking:** Het kan maximaal 24 uur duren voordat de rapportagegegevens voor basislijnen worden weergegeven vanaf de eerste implementatie op een apparaat en tot 6 uur voor verdere updates. 

De meest voorkomende oorzaak voor het niet-toepassen van een basislijninstelling is dat dezelfde instelling in een ander profiel wordt gebruikt. U kunt dit scenario onderzoeken op een specifiek apparaat door dat apparaat te selecteren in het knooppunt Apparaatstatus van het profiel Beveiligingsbasislijnen. Voor meer informatie, zie [Conflicten in beveiligingsbasislijnen oplossen](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).