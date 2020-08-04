---
title: EindpuntDLP configureren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555131"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0b469-102">EindpuntDLP configureren</span><span class="sxs-lookup"><span data-stu-id="0b469-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0b469-103">Met Microsoft Endpoint DLP u de DLP-beveiligings- en bewakingsmogelijkheden uitbreiden naar gevoelige informatie op Windows 10-apparaten.</span><span class="sxs-lookup"><span data-stu-id="0b469-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0b469-104">Nadat apparaten zijn ingeschakeld voor apparaatbeheer, u DLP-beleid maken om beschermende acties voor items af te dwingen.</span><span class="sxs-lookup"><span data-stu-id="0b469-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0b469-105">De Activity Explorer kan worden gebruikt om de activiteit voor gevoelige items te controleren.</span><span class="sxs-lookup"><span data-stu-id="0b469-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0b469-106">Zie [Onboarding-apparaten voor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)meer informatie in apparaatbeheer.</span><span class="sxs-lookup"><span data-stu-id="0b469-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0b469-107">Ga als aan de slag met Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="0b469-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0b469-108">Zorg ervoor dat u over de juiste SKU/abonnementen-licenties beschikt.</span><span class="sxs-lookup"><span data-stu-id="0b469-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0b469-109">Zie [SKU/abonnementen licenties](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0b469-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0b469-110">Controleer de machtigingen die nodig zijn om apparaatbeheer in te schakelen, toegang te krijgen tot de onboarding-pagina of apparaatbewaking in-/uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="0b469-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0b469-111">Zie [Machtigingen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0b469-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0b469-112">Apparaten aan boord in apparaatbeheer door de procedure voor onboarding-apparaten te volgen.</span><span class="sxs-lookup"><span data-stu-id="0b469-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0b469-113">Als u de optie Device Onboarding (preview) mist onder **Nalevingsinstellingen**van M365, bevestigt u dat u de juiste licentie en machtigingen hebt waarnaar hierboven wordt verwezen.</span><span class="sxs-lookup"><span data-stu-id="0b469-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="0b469-114">Zie [Onboarding-apparaten voor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0b469-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0b469-115">Maak DLP-beleid om uw gevoelige items te beschermen.</span><span class="sxs-lookup"><span data-stu-id="0b469-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0b469-116">Zie [Beleidsscenario's voor Eindpunt DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="0b469-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="0b469-117">Zie Informatie over de preventie van [gegevensverlies van Microsoft 365 Endpoint (preview) voor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)meer informatie over de Microsoft Endpoint DLP.</span><span class="sxs-lookup"><span data-stu-id="0b469-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>