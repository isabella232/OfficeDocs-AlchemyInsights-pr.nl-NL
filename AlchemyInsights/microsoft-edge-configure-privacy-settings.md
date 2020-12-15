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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="2d1a4-102">Privacyinstellingen voor Microsoft Edge configureren</span><span class="sxs-lookup"><span data-stu-id="2d1a4-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="2d1a4-103">Als Microsoft Edge op niet-Windows-platforms wordt geïmplementeerd, worden er standaard geen diagnostische gegevens en site-informatie naar Microsoft verzonden.</span><span class="sxs-lookup"><span data-stu-id="2d1a4-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="2d1a4-104">Als Microsoft Edge wordt geïmplementeerd op Windows 10, worden diagnostische gegevens en site-informatie verzonden op basis van de instellingen van de [Windows diagnostische gegevens](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)van gebruikers.</span><span class="sxs-lookup"><span data-stu-id="2d1a4-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="2d1a4-105">Gebruik het volgende groepsbeleid om te configureren hoe gegevensverzameling van Microsoft Edge voor uw organisatie wordt afgehandeld:</span><span class="sxs-lookup"><span data-stu-id="2d1a4-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="2d1a4-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): met dit beleid kunt u informatie over het gebruik en vastlopen van gegevens rapporteren.</span><span class="sxs-lookup"><span data-stu-id="2d1a4-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="2d1a4-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): met dit beleid verzendt u sitegegevens die worden gebruikt om de Microsoft-services te verbeteren.</span><span class="sxs-lookup"><span data-stu-id="2d1a4-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="2d1a4-108">Zie [beleidsinstellingen configureren](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2d1a4-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>