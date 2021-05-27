---
title: Softwarevoorraad ontbreekt of is onjuist
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
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676268"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="ee45a-102">Softwarevoorraad ontbreekt of is onjuist</span><span class="sxs-lookup"><span data-stu-id="ee45a-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="ee45a-103">De softwarevoorraad in Threat and Vulnerability Management (TVM) is een lijst met bekende software in uw organisatie met de officiële Common Platform Enumerations (CPE).</span><span class="sxs-lookup"><span data-stu-id="ee45a-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="ee45a-104">Softwareproducten zonder een officiële CPE hebben geen beveiligingslekken gepubliceerd.</span><span class="sxs-lookup"><span data-stu-id="ee45a-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="ee45a-105">De inventaris bevat ook details, zoals de naam van de leverancier, het aantal zwakke punten, bedreigingen en het aantal blootgestelde apparaten.</span><span class="sxs-lookup"><span data-stu-id="ee45a-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="ee45a-106">Softwarewijzigingen op apparaten worden meestal binnen twee uur doorgevoerd in beveiligingsportalen.</span><span class="sxs-lookup"><span data-stu-id="ee45a-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="ee45a-107">Het kan echter soms langer duren.</span><span class="sxs-lookup"><span data-stu-id="ee45a-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="ee45a-108">Er is momenteel geen manier om een synchronisatie af te dwingen. dit is een doorlopend doorlopend onderzoek.</span><span class="sxs-lookup"><span data-stu-id="ee45a-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="ee45a-109">Als u een softwarewijziging hebt aangebracht en de wijziging na 5 uur niet nauwkeurig wordt weerspiegeld in TVM, volgt u de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="ee45a-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="ee45a-110">Controleer de sectie software-bewijs om te begrijpen hoe de software is gedetecteerd.</span><span class="sxs-lookup"><span data-stu-id="ee45a-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="ee45a-111">Zorg ervoor dat de software wordt ondersteund.</span><span class="sxs-lookup"><span data-stu-id="ee45a-111">Make sure that the software is supported.</span></span> <span data-ttu-id="ee45a-112">Software is mogelijk alleen zichtbaar op apparaatniveau, zelfs als deze momenteel niet wordt ondersteund door Threat and Vulnerability Management.</span><span class="sxs-lookup"><span data-stu-id="ee45a-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="ee45a-113">Er zijn echter slechts beperkte gegevens beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="ee45a-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="ee45a-114">Zie Onnauwkeurigheid van rapport voor stappen om de onnauwkeurigheid vanuit de portal [te rapporteren.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="ee45a-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="ee45a-115">**Opmerking:** Het rapporteren van een onnauwkeurigheid vanuit de MDE-portal is een eenwegkanaal naar engineering.</span><span class="sxs-lookup"><span data-stu-id="ee45a-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="ee45a-116">Als het probleem urgent is, opent u een ondersteuningsticket.</span><span class="sxs-lookup"><span data-stu-id="ee45a-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="ee45a-117">Zie Softwarevoorraad - [Threat and Vulnerability Management.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="ee45a-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>