---
title: Problemen met het verwijderen van een offboarded of buiten bedrijf gesteld apparaat uit de apparaatvoorraad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564168"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="b02f1-102">Problemen met het verwijderen van een offboarded of buiten bedrijf gesteld apparaat uit de apparaatvoorraad</span><span class="sxs-lookup"><span data-stu-id="b02f1-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="b02f1-103">Microsoft Defender voor Eindpunt staat momenteel niet toe dat de apparaatrecord van een uitgeschakeld of buiten gebruik gesteld apparaat handmatig wordt verwijderd uit de apparaatvoorraad.</span><span class="sxs-lookup"><span data-stu-id="b02f1-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="b02f1-104">Voor beveiligingsdoeleinden blijft het apparaat tot 180 dagen in de portal staan als een historische record.</span><span class="sxs-lookup"><span data-stu-id="b02f1-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="b02f1-105">De apparaatgegevens worden echter verwijderd op basis van de geconfigureerde bewaarperiode.</span><span class="sxs-lookup"><span data-stu-id="b02f1-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="b02f1-106">**Opmerking:** Een uitgeschakeld of buiten bedrijf gesteld apparaat schakelt na zeven dagen automatisch over naar **inactieve** toestand.</span><span class="sxs-lookup"><span data-stu-id="b02f1-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="b02f1-107">Bovendien worden apparaten die niet actief zijn in de afgelopen 30 dagen, niet mee verwerkt in de gegevens die uw organisatie weerspiegelen Threat and Vulnerability Management blootstellingsscore of Microsoft Secure Score voor apparaten.</span><span class="sxs-lookup"><span data-stu-id="b02f1-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="b02f1-108">Als u bepaalde apparaten nog steeds niet wilt zien in de weergave Apparaatvoorraad, probeert u een apparaatlabel te plaatsen om het buiten bedrijf gesteld apparaat uit de weergave Apparaatvoorraad te filteren.</span><span class="sxs-lookup"><span data-stu-id="b02f1-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="b02f1-109">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="b02f1-109">For more information, see:</span></span>

[<span data-ttu-id="b02f1-110">Offboard-apparaten van de Microsoft Defender for Endpoint-service</span><span class="sxs-lookup"><span data-stu-id="b02f1-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="b02f1-111">Blootstellingsscore in Threat and Vulnerability Management</span><span class="sxs-lookup"><span data-stu-id="b02f1-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="b02f1-112">Ongezonde sensoren in Microsoft Defender voor eindpunt oplossen</span><span class="sxs-lookup"><span data-stu-id="b02f1-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="b02f1-113">Tags effectief gebruiken (deel 1)</span><span class="sxs-lookup"><span data-stu-id="b02f1-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="b02f1-114">Tags effectief gebruiken (deel 2)</span><span class="sxs-lookup"><span data-stu-id="b02f1-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="b02f1-115">Tags effectief gebruiken (deel 3)</span><span class="sxs-lookup"><span data-stu-id="b02f1-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




