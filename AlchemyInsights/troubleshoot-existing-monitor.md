---
title: Problemen met bestaande monitor oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738564"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="191c5-102">Problemen met een bestaande monitor oplossen</span><span class="sxs-lookup"><span data-stu-id="191c5-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="191c5-103">Probeer deze oplossingen voor het oplossen van een monitor.</span><span class="sxs-lookup"><span data-stu-id="191c5-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="191c5-104">**Het beeldscherm van uw monitor vernieuwen:**</span><span class="sxs-lookup"><span data-stu-id="191c5-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="191c5-105">Druk op de volgende toetsen op hetzelfde moment: Windows-toets + CTRL + SHIFT + B. Hiermee wordt de communicatie met uw grafische stuurprogramma vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="191c5-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="191c5-106">Uw monitoren knipperen kortstondig en komen na enkele seconden weer terug.</span><span class="sxs-lookup"><span data-stu-id="191c5-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="191c5-107">**Problemen met monitor hardware oplossen:**</span><span class="sxs-lookup"><span data-stu-id="191c5-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="191c5-108">Ontkoppel de kabel die uw PC verbindt met uw monitor en sluit deze weer aan.</span><span class="sxs-lookup"><span data-stu-id="191c5-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="191c5-109">Koppel alle niet-essentiële apparaten los van uw PC (zoals adapters of dockingstations).</span><span class="sxs-lookup"><span data-stu-id="191c5-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="191c5-110">**Als u onlangs een update op uw PC hebt geïnstalleerd, u het beeldschermstuurprogramma terugdraaien:**</span><span class="sxs-lookup"><span data-stu-id="191c5-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="191c5-111">Selecteer **Start**, typ **Apparaatbeheer**en selecteer **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="191c5-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="191c5-112">Vouw de sectie **beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **Eigenschappen**.</span><span class="sxs-lookup"><span data-stu-id="191c5-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="191c5-113">Navigeer naar de **Driver** tab en selecteer **roll back driver**.</span><span class="sxs-lookup"><span data-stu-id="191c5-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="191c5-114">Opmerking: als dit niet beschikbaar is of grijs wordt weergegeven, selecteert u **Nee** in de onderstaande opties om naar de volgende stap te gaan.</span><span class="sxs-lookup"><span data-stu-id="191c5-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="191c5-115">Mogelijk moet u uw PC opnieuw opstarten voordat deze wijzigingen van kracht worden.</span><span class="sxs-lookup"><span data-stu-id="191c5-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="191c5-116">**Verwijder het beeldschermstuurprogramma en installeer het opnieuw:**</span><span class="sxs-lookup"><span data-stu-id="191c5-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="191c5-117">Selecteer **Start**, typ **Apparaatbeheer**en selecteer **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="191c5-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="191c5-118">Vouw de sectie **beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **apparaat verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="191c5-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="191c5-119">Vink het vakje aan naast **de stuurprogrammasoftware voor dit apparaat verwijderen** en selecteer **verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="191c5-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="191c5-120">Opmerking: mogelijk wordt u gevraagd om de computer in dit stadium opnieuw op te starten.</span><span class="sxs-lookup"><span data-stu-id="191c5-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="191c5-121">Noteer de resterende instructies voordat u opnieuw opstart.</span><span class="sxs-lookup"><span data-stu-id="191c5-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="191c5-122">Open Apparaatbeheer opnieuw.</span><span class="sxs-lookup"><span data-stu-id="191c5-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="191c5-123">Vouw de sectie **beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **stuurprogramma bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="191c5-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="191c5-124">Selecteer **automatisch zoeken naar software voor het bijwerken van Stuurprogramma's** en volg de installatie-instructies.</span><span class="sxs-lookup"><span data-stu-id="191c5-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>