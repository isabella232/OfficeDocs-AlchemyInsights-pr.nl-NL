---
title: Beleid voor toepassingsbescherming
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423429"
---
# <a name="application-protection-policy"></a><span data-ttu-id="600cc-102">Beleid voor toepassingsbescherming</span><span class="sxs-lookup"><span data-stu-id="600cc-102">Application protection policy</span></span>

<span data-ttu-id="600cc-103">Als u nieuw bent bij App (Application Protection Policy), raadpleegt u het overzicht van het [beleid voor app-beveiliging.](https://docs.microsoft.com/intune/apps/app-protection-policy)</span><span class="sxs-lookup"><span data-stu-id="600cc-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="600cc-104">Zie [App-beveiligingsbeleid maken en toewijzen als](https://docs.microsoft.com/intune/app-protection-policies)u app wilt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="600cc-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="600cc-105">Beleidsvereisten voor toepassingsbescherming:</span><span class="sxs-lookup"><span data-stu-id="600cc-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="600cc-106">De gebruiker heeft een Intune- of EMS-licentie.</span><span class="sxs-lookup"><span data-stu-id="600cc-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="600cc-107">De gebruiker behoort tot een groep die is gericht op het beleid voor toepassingsbescherming.</span><span class="sxs-lookup"><span data-stu-id="600cc-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="600cc-108">Slechts één zakelijke gebruiker is aangemeld bij beveiligde apps op een apparaat.</span><span class="sxs-lookup"><span data-stu-id="600cc-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="600cc-109">De applicatie heeft de [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="600cc-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="600cc-110">Zie Beveiligde Apps van [Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps)voor een lijst met apps die de SDK ondersteunen.</span><span class="sxs-lookup"><span data-stu-id="600cc-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="600cc-111">Het beleid is van toepassing nadat een gebruiker die aan de bovenstaande vereisten voldoet, zich aanmeldt bij een intune SDK-app.</span><span class="sxs-lookup"><span data-stu-id="600cc-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="600cc-112">De eenvoudigste manier om te bepalen of een beleid wordt toegepast, is door te eisen dat de gebruiker een pin in het beleid instelt.</span><span class="sxs-lookup"><span data-stu-id="600cc-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="600cc-113">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="600cc-113">For more information, see:</span></span>

[<span data-ttu-id="600cc-114">VEELGESTELDE VRAGEN OVER HET oplossen VAN APP/MAM-problemen</span><span class="sxs-lookup"><span data-stu-id="600cc-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="600cc-115">De installatie van uw app-beveiligingsbeleid valideren</span><span class="sxs-lookup"><span data-stu-id="600cc-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="600cc-116">De levertijd van app-beveiligingsbeleid begrijpen</span><span class="sxs-lookup"><span data-stu-id="600cc-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="600cc-117">Het beveiligingsbeleid voor apps controleren</span><span class="sxs-lookup"><span data-stu-id="600cc-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)