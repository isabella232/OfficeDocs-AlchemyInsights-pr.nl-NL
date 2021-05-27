---
title: De status van de Defender Endpoint-sensor controleren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676098"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="03c99-102">De status van de Defender Endpoint-sensor controleren</span><span class="sxs-lookup"><span data-stu-id="03c99-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="03c99-103">De **tegel Apparaten met sensorproblemen** bevindt zich op het dashboard Beveiligingsbewerkingen.</span><span class="sxs-lookup"><span data-stu-id="03c99-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="03c99-104">Deze tegel bevat informatie over de mogelijkheid van het afzonderlijke apparaat om sensorgegevens te verstrekken en te communiceren met de Defender for Endpoint-service.</span><span class="sxs-lookup"><span data-stu-id="03c99-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="03c99-105">Het rapport geeft aan hoeveel apparaten aandacht nodig hebben en helpt u problematische apparaten te identificeren en actie te ondernemen om bekende problemen op te lossen.</span><span class="sxs-lookup"><span data-stu-id="03c99-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="03c99-106">Twee statusindicatoren op de tegel geven informatie over het aantal apparaten dat niet correct rapporteert aan de service:</span><span class="sxs-lookup"><span data-stu-id="03c99-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="03c99-107">**Verkeerd geconfigureerd** Apparaten die mogelijk gedeeltelijk sensorgegevens rapporteren aan de Defender for Endpoint-service en mogelijk configuratiefouten hebben die moeten worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="03c99-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="03c99-108">**Inactief** Apparaten die de afgelopen maand meer dan zeven dagen zijn gestopt met rapporteren aan de Defender voor Eindpunt-service.</span><span class="sxs-lookup"><span data-stu-id="03c99-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="03c99-109">Als u op een van de groepen klikt, gaat u naar de lijst Apparaten, gefilterd op basis van uw keuzes.</span><span class="sxs-lookup"><span data-stu-id="03c99-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="03c99-110">In de lijst Apparaten kunt u de lijst met statusstatussen filteren op de volgende status:</span><span class="sxs-lookup"><span data-stu-id="03c99-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="03c99-111">**Actief** Apparaten die actief rapporteren aan de Defender for Endpoint-service.</span><span class="sxs-lookup"><span data-stu-id="03c99-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="03c99-112">**Verkeerd geconfigureerd** Apparaten die mogelijk gedeeltelijk sensorgegevens rapporteren aan de Defender voor Eindpunt-service, maar configuratiefouten hebben die moeten worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="03c99-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="03c99-113">Verkeerd geconfigureerde apparaten kunnen een of een combinatie van de volgende problemen hebben:</span><span class="sxs-lookup"><span data-stu-id="03c99-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="03c99-114">Geen sensorgegevens: apparaten zijn gestopt met het verzenden van sensorgegevens.</span><span class="sxs-lookup"><span data-stu-id="03c99-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="03c99-115">Beperkte waarschuwingen kunnen worden geactiveerd vanaf het apparaat.</span><span class="sxs-lookup"><span data-stu-id="03c99-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="03c99-116">Communicatie met een beperking: de mogelijkheid om te communiceren met een apparaat is beperkt.</span><span class="sxs-lookup"><span data-stu-id="03c99-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="03c99-117">Het verzenden van bestanden voor uitgebreide analyse, het blokkeren van bestanden, het isoleren van apparaten van het netwerk en andere acties waarvoor communicatie met het apparaat is vereist, werkt mogelijk niet.</span><span class="sxs-lookup"><span data-stu-id="03c99-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="03c99-118">**Inactief** Apparaten die niet meer rapporteren aan de Defender voor Eindpunt-service.</span><span class="sxs-lookup"><span data-stu-id="03c99-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="03c99-119">U kunt de hele lijst downloaden in CSV-indeling met de functie Exporteren.</span><span class="sxs-lookup"><span data-stu-id="03c99-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="03c99-120">Zie De status van [de sensor controleren in Microsoft Defender voor eindpunt voor meer informatie.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="03c99-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="03c99-121">Zie Ongezonde sensoren in Microsoft Defender voor eindpunt oplossen voor meer informatie over de oorzaak van inactiviteit of onjuiste configuratie van [een apparaat.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="03c99-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
