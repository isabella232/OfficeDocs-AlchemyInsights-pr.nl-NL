---
title: Problemen met het onboarden van Windows 10-apparaten op afstand oplossen met Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744721"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="0b8ce-102">Problemen met het onboarden van Windows 10-apparaten op afstand oplossen met Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="0b8ce-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="0b8ce-103">Als u toegang hebt tot de externe computer, volgt u de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="0b8ce-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="0b8ce-104">Download het [diagnostische hulpprogramma Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="0b8ce-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="0b8ce-105">Haal MDATPAnalyzer.cmd op en voer deze uit.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="0b8ce-106">Zoek het diagnostische logboek in de map MDATPClientAnalyzerResult, dezelfde map waarin het hulpprogramma Analyzer is gedownload.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="0b8ce-107">Als u problemen wilt zoeken met de connectiviteits- of internetproxyinstellingen, bekijkt u de logboekbestandsinstellingen MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="0b8ce-108">Zie Problemen met [onboarding-machines](https://go.microsoft.com/fwlink/?linkid=2143634)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
