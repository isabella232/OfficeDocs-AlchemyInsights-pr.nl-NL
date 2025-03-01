---
title: DLP-licentiefout eindpunt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322126"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpoint DLP-licentiefout

Als u endpoint DLP probeert in te stellen, krijgt u de volgende foutmelding:

`Your organization is missing the licenses required to manage these devices`.

Zorg ervoor dat u een van de volgende abonnementen of invoegtoepassingen hebt:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 Information Protection en governance
- Microsoft 365 A5 Information Protection en governance

**Opmerking:** Dit werkt niet voor licentiecombinaties zoals: Win E5 + O365 E5 + EMS E5. U moet een pure M365 E5-licentie hebben om deze functie in te stellen.

Zie Endpoint DLP Licensing (Endpoint DLP Licensing) voor meer informatie over [endpoint-DLP-licenties.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
