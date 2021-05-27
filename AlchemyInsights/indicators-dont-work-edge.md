---
title: Indicatoren werken niet met de Edge-browser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676244"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="37fde-102">Indicatoren werken niet met de Edge-browser</span><span class="sxs-lookup"><span data-stu-id="37fde-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="37fde-103">Nadat u een indicator hebt gemaakt, wordt deze niet geëerd door Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="37fde-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="37fde-104">Zie Indicatoren maken [voor IPs en URL's/domeinen voor meer informatie.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="37fde-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="37fde-105">Stap 1: Controleer het volgende</span><span class="sxs-lookup"><span data-stu-id="37fde-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="37fde-106">Controleer of de indicator juist is (geen typfouten in IP/URL, juiste actie, de juiste RBAC-groepen).</span><span class="sxs-lookup"><span data-stu-id="37fde-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="37fde-107">Wacht minimaal 2 uur na het maken van de indicator om rekening te houden met eventuele latentie.</span><span class="sxs-lookup"><span data-stu-id="37fde-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="37fde-108">Controleer of het systeem(en) zijn onboarded bij Microsoft Defender voor Eindpunt.</span><span class="sxs-lookup"><span data-stu-id="37fde-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="37fde-109">Controleer of systeem(en) kunnen communiceren met de cloud.</span><span class="sxs-lookup"><span data-stu-id="37fde-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="37fde-110">Controleer of Smartscreen is ingeschakeld en bereikbaar is door naar de [testsite te gaan.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="37fde-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="37fde-111">Stap 2: Het mogelijke probleem oplossen</span><span class="sxs-lookup"><span data-stu-id="37fde-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="37fde-112">Zorg ervoor dat de client aan de vereisten voldoet.</span><span class="sxs-lookup"><span data-stu-id="37fde-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="37fde-113">Zie Indicatoren maken [voor IPs en URL's/domeinen voor meer informatie.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="37fde-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="37fde-114">Zorg ervoor dat u de nieuwste versie van de Edge-browser gebruikt.</span><span class="sxs-lookup"><span data-stu-id="37fde-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="37fde-115">Zie Welke versie van de Microsoft Edge u hebt voor meer informatie over de meest [recente versie.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="37fde-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="37fde-116">Start de Edge-browser opnieuw.</span><span class="sxs-lookup"><span data-stu-id="37fde-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="37fde-117">Ga naar de site waarvoor u een indicator hebt ingesteld.</span><span class="sxs-lookup"><span data-stu-id="37fde-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="37fde-118">Als de site niet wordt weergegeven zoals verwacht, gaat u verder met stap 3.</span><span class="sxs-lookup"><span data-stu-id="37fde-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="37fde-119">Stap 3: Gegevens verzamelen</span><span class="sxs-lookup"><span data-stu-id="37fde-119">Step 3: Collect data</span></span>

- <span data-ttu-id="37fde-120">**MDEClientAnalyzer-diagnostische** gegevens verzamelen.</span><span class="sxs-lookup"><span data-stu-id="37fde-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="37fde-121">Zie Problemen met [onboarding-machines](issues-with-onboarding-machines.md)bij Microsoft Defender voor Eindpunt voor instructies.</span><span class="sxs-lookup"><span data-stu-id="37fde-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="37fde-122">Zie [Telerik Fiddler](http://www.telerik.com/fiddler)als u vertrouwd bent met het installeren en verzamelen van een Fiddler-trace.</span><span class="sxs-lookup"><span data-stu-id="37fde-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="37fde-123">Als u de voorkeur geeft aan ondersteuning van Microsoft Support, selecteert u het pictogram Ondersteuning hieronder om een ondersteuningscase te openen.</span><span class="sxs-lookup"><span data-stu-id="37fde-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
