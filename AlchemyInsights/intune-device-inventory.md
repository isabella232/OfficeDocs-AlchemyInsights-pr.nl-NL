---
title: Inventaris van intune-apparaten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439159"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="fddeb-102">Inventaris van intune-apparaten</span><span class="sxs-lookup"><span data-stu-id="fddeb-102">Intune Device Inventory</span></span>

<span data-ttu-id="fddeb-103">Het apparaat van de apparaten geeft de beheerder inzicht in apparaten die onder beheer zijn in Intune per apparaat.</span><span class="sxs-lookup"><span data-stu-id="fddeb-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="fddeb-104">De getoonde informatie omvat: Hardware, Gedetecteerde toepassingen, status apparaatnaleving en status apparaatconfiguratie.</span><span class="sxs-lookup"><span data-stu-id="fddeb-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="fddeb-105">Voorraadgegevens voor hardware en gedetecteerde toepassingen worden verzameld op een cyclus van zeven dagen.</span><span class="sxs-lookup"><span data-stu-id="fddeb-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="fddeb-106">De toepassingen en specifieke elementen van de gerapporteerde hardware verschillen afhankelijk van het besturingssysteem van het apparaat en of het apparaat persoonlijk of eigendom van het bedrijf is.</span><span class="sxs-lookup"><span data-stu-id="fddeb-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="fddeb-107">[Zie Apparaatgegevens in Intune voor](https://docs.microsoft.com/intune/device-inventory)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fddeb-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="fddeb-108">**Veelgestelde vragen**</span><span class="sxs-lookup"><span data-stu-id="fddeb-108">**FAQ**</span></span>

<span data-ttu-id="fddeb-109">V: Ik ontvang geen volledige voorraadlijst van toepassingen die aanwezig zijn op Intune-ingeschreven Windows-apparaten.</span><span class="sxs-lookup"><span data-stu-id="fddeb-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="fddeb-110">Waarom niet?</span><span class="sxs-lookup"><span data-stu-id="fddeb-110">Why not?</span></span>

<span data-ttu-id="fddeb-111">A: Op dit moment worden alleen moderne apps weergegeven voor Windows 10-pc's die zijn geïdentificeerd als bedrijfsapparaten.</span><span class="sxs-lookup"><span data-stu-id="fddeb-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="fddeb-112">Intune verzamelt geen informatie over Win32-apps die op deze apparaten zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="fddeb-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="fddeb-113">V: Waarom worden telefoonnummers niet verzameld van alle apparaten?</span><span class="sxs-lookup"><span data-stu-id="fddeb-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="fddeb-114">A: Telefoons die zijn gecategoriseerd als bedrijfsapparaten in Intune, worden niet geïdentificeerd met hun volledige telefoonnummer wanneer u bijvoorbeeld een inventarisrapport voor mobiele apparaten uitvoert.</span><span class="sxs-lookup"><span data-stu-id="fddeb-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="fddeb-115">Telefoonnummers voor bring-you-own-device worden altijd gedeeltelijk gemaskeerd met sterretjes (\*\*\*\*), en tonen alleen de laatste vier cijfers.</span><span class="sxs-lookup"><span data-stu-id="fddeb-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>