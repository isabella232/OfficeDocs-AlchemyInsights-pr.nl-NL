---
title: Privacyinstellingen voor Microsoft Edge configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677250"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Privacyinstellingen voor Microsoft Edge configureren

Als Microsoft Edge op niet-Windows-platforms wordt geïmplementeerd, worden er standaard geen diagnostische gegevens en site-informatie naar Microsoft verzonden. Als Microsoft Edge wordt geïmplementeerd op Windows 10, worden diagnostische gegevens en site-informatie verzonden op basis van de instellingen van de [Windows diagnostische gegevens](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)van gebruikers.

Gebruik het volgende groepsbeleid om te configureren hoe gegevensverzameling van Microsoft Edge voor uw organisatie wordt afgehandeld:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): met dit beleid kunt u informatie over het gebruik en vastlopen van gegevens rapporteren.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): met dit beleid verzendt u sitegegevens die worden gebruikt om de Microsoft-services te verbeteren.

Zie [beleidsinstellingen configureren](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)voor meer informatie.