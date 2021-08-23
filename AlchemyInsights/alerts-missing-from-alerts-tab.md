---
title: Waarschuwingen ontbreken op het tabblad Waarschuwingen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454533"
---
# <a name="alerts-missing-from-alerts-tab"></a>Waarschuwingen ontbreken op het tabblad Waarschuwingen

Het **tabblad Waarschuwingen** werkt op basis van het installatie- en geactiveerde beleid vanuit de app-beheerportal in uw tenant. Out-of-the-box-beleid in App-beheer moet ook worden geactiveerd om signalen naar het tabblad **Waarschuwingen te laten** stromen. 

Controleer of de waarschuwing is gegenereerd:

1. Ga naar beleid [voor](https://compliance.microsoft.com/m365appprotection?viewid=policies) app-beheer en bevestig dat u ten minste één actief of auditbeleid hebt gemaakt.

1. Selecteer het beleid en seleect **Bewerken** in het deelvenster Flyout. 

1. Controleer de beleidsconfiguratie om te controleren of er een waarschuwing moet zijn gegenereerd op basis van een beleidsgebeurtenis die meer dan 24 uur geleden is gestart.

Zie Aan de slag met [](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)detectie en herstel van app-bedreigingen voor meer informatie over waarschuwingen in App Governance.