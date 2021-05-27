---
title: Problemen met ediscovery oplossen bevat fouten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676085"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Problemen met ediscovery oplossen bevat fouten

Ondervindt u problemen met eDiscovery-bezit? Hier volgen enkele best practices om rekening mee te houden:

- Controleer de distributiestatus van de wacht.  Als de status **Aan (In behandeling)** of **Uit (In behandeling)** is, wacht u totdat de distributie in de wacht is gezet.
- EDiscovery-holdupdates samenvoegen in één bulkaanvraag in plaats van het beleid herhaaldelijk bij te werken voor elke transactie.
- Voer Set-CaseHoldPolicy <policyname> -RetryDistribution uit in het Powershell-beveiligings- en compliancecentrum. Zie Verbinding maken & PowerShell voor [meer informatie.](/powershell/exchange/connect-to-scc-powershell)

Zie Problemen met eDiscovery oplossen voor stappen om deze instellingen en aanvullende best practices voor het voorkomen en oplossen van problemen met [eDiscovery te controleren.](/microsoft-365/compliance/hold-distribution-errors)
Zie Veelvoorkomende eDiscovery-problemen onderzoeken, oplossen en oplossen voor informatie over het oplossen van andere veelvoorkomende [eDiscovery-problemen.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
