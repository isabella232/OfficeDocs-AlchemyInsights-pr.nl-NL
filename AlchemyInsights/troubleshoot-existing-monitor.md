---
title: Problemen oplossen met bestaande monitor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690706"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="9075e-102">Problemen met een bestaande monitor oplossen</span><span class="sxs-lookup"><span data-stu-id="9075e-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="9075e-103">Probeer deze oplossingen om problemen op te lossen met een beeldscherm.</span><span class="sxs-lookup"><span data-stu-id="9075e-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="9075e-104">**De weergave van het beeldscherm vernieuwen:**</span><span class="sxs-lookup"><span data-stu-id="9075e-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="9075e-105">Druk op de volgende toetsen tegelijk: Windows-toets + CTRL + SHIFT + B. Hiermee wordt de communicatie met uw grafische stuurprogramma vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="9075e-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="9075e-106">Uw monitoren knipperen en werken na een paar seconden opnieuw.</span><span class="sxs-lookup"><span data-stu-id="9075e-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="9075e-107">**Problemen met monitor-hardware oplossen:**</span><span class="sxs-lookup"><span data-stu-id="9075e-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="9075e-108">Ontkoppel de kabel die uw PC verbindt met uw monitor en sluit de kabel weer aan.</span><span class="sxs-lookup"><span data-stu-id="9075e-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="9075e-109">Verbreek de verbinding van niet-essentiële apparaten vanaf uw PC (zoals adapters en docks).</span><span class="sxs-lookup"><span data-stu-id="9075e-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="9075e-110">**Als u onlangs een update op uw PC hebt geïnstalleerd, kunt u het beeldschermstuurprogramma herstellen:**</span><span class="sxs-lookup"><span data-stu-id="9075e-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="9075e-111">Selecteer **Start**, typ **Apparaatbeheer**en kies **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="9075e-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="9075e-112">Vouw de sectie **weergave-adapters** uit, klik met de rechtermuisknop op de beeldschermadapter, ands Selecteer **Eigenschappen**.</span><span class="sxs-lookup"><span data-stu-id="9075e-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="9075e-113">Ga naar het tabblad **stuurprogramma** en selecteer vorig **stuurprogramma terugdraaien**.</span><span class="sxs-lookup"><span data-stu-id="9075e-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="9075e-114">Opmerking: als dit niet beschikbaar is of niet beschikbaar is, selecteert u **Nee** in de onderstaande opties om naar de volgende stap te gaan.</span><span class="sxs-lookup"><span data-stu-id="9075e-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="9075e-115">Mogelijk moet u de PC opnieuw opstarten voordat de wijzigingen van kracht worden.</span><span class="sxs-lookup"><span data-stu-id="9075e-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="9075e-116">**Het beeldschermstuurprogramma verwijderen en opnieuw installeren:**</span><span class="sxs-lookup"><span data-stu-id="9075e-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="9075e-117">Selecteer **Start**, typ **Apparaatbeheer**en kies **Apparaatbeheer** in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="9075e-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="9075e-118">Vouw de sectie **weergave-adapters** uit, klik met de rechtermuisknop op de beeldschermadapter, ands Selecteer **apparaat verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="9075e-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="9075e-119">Schakel het selectievakje in naast **de stuurprogrammasoftware voor dit apparaat verwijderen** en selecteer **verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="9075e-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="9075e-120">Opmerking: u wordt mogelijk gevraagd om de computer in deze fase opnieuw op te starten.</span><span class="sxs-lookup"><span data-stu-id="9075e-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="9075e-121">Noteer de overige instructies voordat u de computer opnieuw opstart.</span><span class="sxs-lookup"><span data-stu-id="9075e-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="9075e-122">Open Apparaatbeheer opnieuw.</span><span class="sxs-lookup"><span data-stu-id="9075e-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="9075e-123">Vouw de sectie **weergave-adapters** uit, klik met de rechtermuisknop op de beeldschermadapter en selecteer **Driver bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="9075e-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="9075e-124">Selecteer **automatisch zoeken naar Stuurprogrammasoftware bijwerken** en volg de installatie-instructies.</span><span class="sxs-lookup"><span data-stu-id="9075e-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>