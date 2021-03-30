---
title: Eindpunt-DLP configureren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402412"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f51bd-102">Eindpunt-DLP configureren</span><span class="sxs-lookup"><span data-stu-id="f51bd-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f51bd-103">Met Microsoft Eindpunt-DLP kunt u de DLP-beveiliging en -controle uitbreiden naar gevoelige informatie op Windows 10-apparaten.</span><span class="sxs-lookup"><span data-stu-id="f51bd-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f51bd-104">Nadat apparaten in gebruik zijn genomen bij apparaatbeheer, kunt u DLP-beleid maken om beschermende acties op items af te dwingen.</span><span class="sxs-lookup"><span data-stu-id="f51bd-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f51bd-105">De Activiteitenverkenner kan worden gebruikt om activiteiten voor gevoelige items te bewaken.</span><span class="sxs-lookup"><span data-stu-id="f51bd-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f51bd-106">Zie [Onboarding van apparaten in apparaatbeheer](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f51bd-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f51bd-107">Aan de slag met Eindpunt-DLP:</span><span class="sxs-lookup"><span data-stu-id="f51bd-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f51bd-108">Zorg ervoor dat u de juiste SKU/abonnementenlicenties hebt.</span><span class="sxs-lookup"><span data-stu-id="f51bd-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f51bd-109">Zie voor meer informatie [SKU/abonnementenlicenties](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f51bd-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f51bd-110">Controleer de vereiste machtigingen om apparaatbeheer in te schakelen, toegang te krijgen tot de onboardingpagina of apparaatcontrole in of uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="f51bd-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f51bd-111">Zie [Machtigingen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f51bd-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f51bd-112">Onboard apparaten in Apparaatbeheer door de onboarding-procedure voor apparaten te volgen.</span><span class="sxs-lookup"><span data-stu-id="f51bd-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f51bd-113">Als de optie Device Onboarding (preview) ontbreekt onder M365 Compliance  **Instellingen**, controleert u of u de juiste licentie en machtigingen hebt waarnaar hierboven is verwezen.</span><span class="sxs-lookup"><span data-stu-id="f51bd-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="f51bd-114">Zie [Onboarding van apparaten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f51bd-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f51bd-115">Maak DLP-beleid ter bescherming van uw gevoelige items.</span><span class="sxs-lookup"><span data-stu-id="f51bd-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f51bd-116">Zie voor meer informatie [DLP-beleidsscenario's voor eindpunten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f51bd-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="f51bd-117">Zie [Meer informatie over preventie van gegevensverlies voor Microsoft 365-eindpunten (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f51bd-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f51bd-118">**Belangrijke stappen voor het verzamelen van gegevens, als ondersteuning nodig is:**</span><span class="sxs-lookup"><span data-stu-id="f51bd-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f51bd-119">MDATP Client Analyzer Preview downloaden vanuit [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="f51bd-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="f51bd-120">Voer het hulpprogramma als beheerder uit vanuit het cmd-venster:</span><span class="sxs-lookup"><span data-stu-id="f51bd-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="f51bd-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="f51bd-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="f51bd-122">Wanneer u wordt gevraagd het aantal minuten voor het verzamelen van traceringen in te voeren: ", voer het aantal minuten in dat nodig is om het scenario uit te voeren</span><span class="sxs-lookup"><span data-stu-id="f51bd-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="f51bd-123">Het scenario uitvoeren</span><span class="sxs-lookup"><span data-stu-id="f51bd-123">Run the scenario</span></span>

<span data-ttu-id="f51bd-124">Verzamel de uitvoer van het ZIP-bestand dat aan de ondersteuningsagent moet worden gegeven.</span><span class="sxs-lookup"><span data-stu-id="f51bd-124">Collect the Zip file output to be given to the Support agent.</span></span>
