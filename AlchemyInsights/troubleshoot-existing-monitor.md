---
title: Problemen met bestaande monitor oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824574"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="89ab8-102">Problemen met een bestaande monitor oplossen</span><span class="sxs-lookup"><span data-stu-id="89ab8-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="89ab8-103">Probeer deze oplossingen om problemen met een monitor op te lossen.</span><span class="sxs-lookup"><span data-stu-id="89ab8-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="89ab8-104">**Het beeldscherm vernieuwen:**</span><span class="sxs-lookup"><span data-stu-id="89ab8-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="89ab8-105">Druk tegelijkertijd op de volgende toetsen: Windows-toets + Ctrl + Shift + B. Hierdoor wordt de communicatie met het grafische stuurprogramma vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="89ab8-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="89ab8-106">Uw beeldschermen knipperen tijdelijk en komen na enkele seconden terug.</span><span class="sxs-lookup"><span data-stu-id="89ab8-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="89ab8-107">**Problemen met monitorhardware oplossen:**</span><span class="sxs-lookup"><span data-stu-id="89ab8-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="89ab8-108">Loskoppel de kabel die uw pc verbindt met uw monitor en sluit deze weer aan.</span><span class="sxs-lookup"><span data-stu-id="89ab8-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="89ab8-109">Loskoppelen van niet-essentiële apparaten van uw pc (zoals adapters of docks).</span><span class="sxs-lookup"><span data-stu-id="89ab8-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="89ab8-110">**Als u onlangs een update op uw pc hebt geïnstalleerd, kunt u het display-stuurprogramma terugdraaien:**</span><span class="sxs-lookup"><span data-stu-id="89ab8-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="89ab8-111">Selecteer **Start,** typ **Apparaatbeheer** en selecteer **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="89ab8-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="89ab8-112">Vouw de **sectie Beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **Eigenschappen.**</span><span class="sxs-lookup"><span data-stu-id="89ab8-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="89ab8-113">Ga naar het **tabblad Stuurprogramma** en selecteer **Stuurprogramma terugdraaien.**</span><span class="sxs-lookup"><span data-stu-id="89ab8-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="89ab8-114">Opmerking: Als dit niet beschikbaar is of niet beschikbaar is, selecteert u Nee **in** de onderstaande opties om naar de volgende stap te gaan.</span><span class="sxs-lookup"><span data-stu-id="89ab8-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="89ab8-115">Mogelijk moet u uw pc opnieuw opstarten voordat deze wijzigingen van kracht worden.</span><span class="sxs-lookup"><span data-stu-id="89ab8-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="89ab8-116">**Verwijder en installeer het beeldschermstuur stuurprogramma:**</span><span class="sxs-lookup"><span data-stu-id="89ab8-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="89ab8-117">Selecteer **Start,** typ **Apparaatbeheer** en selecteer **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="89ab8-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="89ab8-118">Vouw de **sectie Beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **Apparaat verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="89ab8-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="89ab8-119">Schakel het vakje naast **De stuurprogrammasoftware voor** dit apparaat verwijderen in en selecteer **Verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="89ab8-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="89ab8-120">Opmerking: mogelijk wordt u gevraagd uw computer in dit stadium opnieuw op te starten.</span><span class="sxs-lookup"><span data-stu-id="89ab8-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="89ab8-121">Schrijf de resterende instructies op voordat u opnieuw start.</span><span class="sxs-lookup"><span data-stu-id="89ab8-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="89ab8-122">Open Device Manager opnieuw.</span><span class="sxs-lookup"><span data-stu-id="89ab8-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="89ab8-123">Vouw de **sectie Beeldschermadapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **Stuurprogramma bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="89ab8-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="89ab8-124">Selecteer **Automatisch zoeken naar software voor het bijwerken van stuurprogramma's** en volg de installatie-instructies.</span><span class="sxs-lookup"><span data-stu-id="89ab8-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>