---
title: Verloren iOS-apparaten lokaliseren met Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439143"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="3c861-102">Verloren iOS-apparaten lokaliseren met Intune</span><span class="sxs-lookup"><span data-stu-id="3c861-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="3c861-103">Als u de verloren modus op een iOS-apparaat inschakelt, kan een beheerder een bericht en telefoonnummer op het vergrendelingsscherm weergeven.</span><span class="sxs-lookup"><span data-stu-id="3c861-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="3c861-104">Nadat de verloren modus is ingeschakeld, kan de beheerder de actie Apparaat lokaliseren gebruiken om de fysieke locatie van het apparaat te identificeren.</span><span class="sxs-lookup"><span data-stu-id="3c861-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="3c861-105">De actie Apparaat zoeken in Intune werkt met iOS-apparaten om de locatie van een specifiek apparaat op een kaart weer te geven.</span><span class="sxs-lookup"><span data-stu-id="3c861-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="3c861-106">Voor het gebruik van deze actie moet het iOS-apparaat zich in:</span><span class="sxs-lookup"><span data-stu-id="3c861-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="3c861-107">Bewaakte modus</span><span class="sxs-lookup"><span data-stu-id="3c861-107">Supervised mode</span></span>
- <span data-ttu-id="3c861-108">Verloren modus</span><span class="sxs-lookup"><span data-stu-id="3c861-108">Lost mode</span></span>

<span data-ttu-id="3c861-109">Zie [Verloren modus inschakelen op iOS/iPadOS-apparaten met Intune](https://docs.microsoft.com/intune/device-lost-mode) en Verloren verloren [iOS/iPadOS-apparaten lokaliseren met Intune](https://docs.microsoft.com/intune/device-locate)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="3c861-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="3c861-110">**Veelgestelde vragen**</span><span class="sxs-lookup"><span data-stu-id="3c861-110">**FAQ**</span></span>

<span data-ttu-id="3c861-111">V: Ik heb een actie op afstand uitgevaardigd om bedrijfsgegevens van een apparaat te verwijderen en nu zit deze vast in een in behandeling zijnde status.</span><span class="sxs-lookup"><span data-stu-id="3c861-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="3c861-112">A: Om een actie op afstand succesvol te voltooien, moet het beoogde apparaat online en gezond zijn.</span><span class="sxs-lookup"><span data-stu-id="3c861-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="3c861-113">In de volgende situaties blijft de actie op afstand 30 dagen in behandeling of totdat het apparaat de opdracht erkent:</span><span class="sxs-lookup"><span data-stu-id="3c861-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="3c861-114">Wanneer het apparaat geen verbinding heeft</span><span class="sxs-lookup"><span data-stu-id="3c861-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="3c861-115">Wanneer het apparaat zijn beheerstatus verliest met Intune</span><span class="sxs-lookup"><span data-stu-id="3c861-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="3c861-116">Als u denkt dat een apparaat niet meer incheckt en als het bedrijfsgegevens niet kan verwijderen, selecteert u Verwijderen.</span><span class="sxs-lookup"><span data-stu-id="3c861-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="3c861-117">Als u de apparaatrecord verwijdert, wordt de apparaatrecord verwijderd, zodat deze niet meer wordt weergegeven in de Intune-lijst met apparaten.</span><span class="sxs-lookup"><span data-stu-id="3c861-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="3c861-118">Als het apparaat weer actief wordt, moet de gebruiker het opnieuw inschrijven.</span><span class="sxs-lookup"><span data-stu-id="3c861-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="3c861-119">V: Waarom zijn bepaalde acties op afstand niet beschikbaar voor mij om te gebruiken?</span><span class="sxs-lookup"><span data-stu-id="3c861-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="3c861-120">A: Niet alle platforms ondersteunen alle acties op afstand.</span><span class="sxs-lookup"><span data-stu-id="3c861-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="3c861-121">De volgende externe acties zijn platformspecifiek, dus ze zijn alleen beschikbaar voor de genoemde platforms.</span><span class="sxs-lookup"><span data-stu-id="3c861-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="3c861-122">Activeringsvergrendeling omzeilen (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="3c861-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="3c861-123">Nieuwe start (alleen Windows)</span><span class="sxs-lookup"><span data-stu-id="3c861-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="3c861-124">Verloren modus (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="3c861-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="3c861-125">Apparaat zoeken (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="3c861-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="3c861-126">Opnieuw opstarten (alleen Windows)</span><span class="sxs-lookup"><span data-stu-id="3c861-126">Restart (Windows only)</span></span>

<span data-ttu-id="3c861-127">Zie Acties voor beschikbare [apparaten](https://docs.microsoft.com/intune/device-management#available-device-actions)voor meer informatie over elke actie.</span><span class="sxs-lookup"><span data-stu-id="3c861-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>