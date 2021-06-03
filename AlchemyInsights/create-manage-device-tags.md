---
title: Apparaatlabels of -groepen maken en beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731449"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="fcc72-102">Apparaatlabels of -groepen maken en beheren</span><span class="sxs-lookup"><span data-stu-id="fcc72-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="fcc72-103">Voeg tags toe aan apparaten om een logische groep te maken.</span><span class="sxs-lookup"><span data-stu-id="fcc72-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="fcc72-104">Apparaatlabels ondersteunen de juiste toewijzing van het netwerk, zodat u verschillende tags kunt koppelen om context vast te leggen en dynamische lijstcreatie als onderdeel van een incident kunt inschakelen.</span><span class="sxs-lookup"><span data-stu-id="fcc72-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="fcc72-105">Tags kunnen worden gebruikt als filter in de lijstweergave Apparaten of om apparaten te groeperen.</span><span class="sxs-lookup"><span data-stu-id="fcc72-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="fcc72-106">Zie Apparaatlabels maken en beheren voor meer informatie over [apparaatgroepering.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="fcc72-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="fcc72-107">U kunt tags toevoegen op apparaten door:</span><span class="sxs-lookup"><span data-stu-id="fcc72-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="fcc72-108">De portal gebruiken</span><span class="sxs-lookup"><span data-stu-id="fcc72-108">Using the portal</span></span>

- <span data-ttu-id="fcc72-109">Een registersleutelwaarde instellen</span><span class="sxs-lookup"><span data-stu-id="fcc72-109">Setting a registry key value</span></span>
 
<span data-ttu-id="fcc72-110">**Opmerking:** Er kan latentie zijn tussen het moment dat een tag wordt toegevoegd aan een apparaat en de beschikbaarheid ervan in de lijst met apparaten en de apparaatpagina.</span><span class="sxs-lookup"><span data-stu-id="fcc72-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="fcc72-111">Zie Api voor apparaatlabels toevoegen of verwijderen als u apparaatlabels wilt toevoegen met [API.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="fcc72-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="fcc72-112">Apparaatlabels toevoegen en beheren met de portal</span><span class="sxs-lookup"><span data-stu-id="fcc72-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="fcc72-113">Selecteer het apparaat waar u tags op wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="fcc72-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="fcc72-114">U kunt een apparaat selecteren of zoeken in een van de volgende weergaven:</span><span class="sxs-lookup"><span data-stu-id="fcc72-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="fcc72-115">**Dashboard Beveiligingsbewerkingen** Selecteer de naam van het apparaat in de sectie Topapparaten met actieve waarschuwingen.</span><span class="sxs-lookup"><span data-stu-id="fcc72-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="fcc72-116">**Waarschuwingenwachtrij:** selecteer de naam van het apparaat naast het apparaatpictogram in de waarschuwingenwachtrij.</span><span class="sxs-lookup"><span data-stu-id="fcc72-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="fcc72-117">**Lijst met** apparaten: selecteer de naam van het apparaat in de lijst met apparaten.</span><span class="sxs-lookup"><span data-stu-id="fcc72-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="fcc72-118">**Zoekvak:** selecteer Apparaat in de vervolgkeuzelijst en voer de naam van het apparaat in.</span><span class="sxs-lookup"><span data-stu-id="fcc72-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="fcc72-119">U kunt ook naar de waarschuwingspagina gaan via de bestands- en IP-weergaven.</span><span class="sxs-lookup"><span data-stu-id="fcc72-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="fcc72-120">Selecteer **Tags beheren** in de rij met antwoordacties.</span><span class="sxs-lookup"><span data-stu-id="fcc72-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="fcc72-121">Typ om tags te zoeken of te maken.</span><span class="sxs-lookup"><span data-stu-id="fcc72-121">Type to find or create tags.</span></span>

<span data-ttu-id="fcc72-122">Tags worden toegevoegd aan de apparaatweergave en worden weergegeven in de lijstweergave Apparaten.</span><span class="sxs-lookup"><span data-stu-id="fcc72-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="fcc72-123">Vervolgens kunt u het filter Tags gebruiken om de relevante lijst met apparaten te bekijken.</span><span class="sxs-lookup"><span data-stu-id="fcc72-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="fcc72-124">Zie Apparaatlabels maken en beheren voor meer [informatie.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="fcc72-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>