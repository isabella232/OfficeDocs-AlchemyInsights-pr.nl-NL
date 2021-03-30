---
title: Privacy-instellingen configureren in Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404619"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="f5ee5-102">Privacy-instellingen configureren in Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f5ee5-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="f5ee5-103">Als Microsoft Edge standaard wordt geïmplementeerd op niet-Windows-platforms, worden diagnostische gegevens en sitegegevens niet naar Microsoft verzonden.</span><span class="sxs-lookup"><span data-stu-id="f5ee5-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="f5ee5-104">Als Microsoft Edge echter wordt geïmplementeerd in Windows 10, worden diagnostische gegevens en sitegegevens verzonden op basis van de [windows diagnostische gegevensinstellingen van gebruikers.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="f5ee5-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="f5ee5-105">Als u wilt configureren hoe Microsoft Edge gegevensverzameling voor uw organisatie verwerkt, gebruikt u het volgende groepsbeleid:</span><span class="sxs-lookup"><span data-stu-id="f5ee5-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="f5ee5-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) schakelt rapportage in van gebruiks- en crashgerelateerde gegevens.</span><span class="sxs-lookup"><span data-stu-id="f5ee5-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="f5ee5-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) verzendt sitegegevens die worden gebruikt om Microsoft-services te verbeteren.</span><span class="sxs-lookup"><span data-stu-id="f5ee5-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="f5ee5-108">Zie Beleidsinstellingen [configureren voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="f5ee5-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
