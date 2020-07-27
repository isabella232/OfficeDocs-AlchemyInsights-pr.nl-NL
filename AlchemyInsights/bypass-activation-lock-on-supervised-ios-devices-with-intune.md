---
title: Activeringsvergrendeling omzeilen op iOS-apparaten onder toezicht met Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423489"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="80f11-102">Activeringsvergrendeling omzeilen op iOS-apparaten onder toezicht met Intune</span><span class="sxs-lookup"><span data-stu-id="80f11-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="80f11-103">De mogelijkheid om het activeringsslot op iOS-apparaten te omzeilen, maakt het gemakkelijker om te herstellen van het scenario waarin een gebruiker activeringsvergrendeling op een bedrijfsapparaat inschakelt en verlaat het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="80f11-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="80f11-104">Vereisten voor het omzeilen van een activeringsslot zijn:</span><span class="sxs-lookup"><span data-stu-id="80f11-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="80f11-105">Een apparaat is dat is "gecontroleerd."</span><span class="sxs-lookup"><span data-stu-id="80f11-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="80f11-106">Het activeringsslot is ingeschakeld met het beperkingsbeleid van iOS-apparaten in Intune.</span><span class="sxs-lookup"><span data-stu-id="80f11-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="80f11-107">Bovendien moet u bij het omzeilen van een activeringsslot:</span><span class="sxs-lookup"><span data-stu-id="80f11-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="80f11-108">Fysiek bezit het apparaat wordt gewist.</span><span class="sxs-lookup"><span data-stu-id="80f11-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="80f11-109">Kopieer de code voordat u het wissen uitgave.</span><span class="sxs-lookup"><span data-stu-id="80f11-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="80f11-110">**Let op:** De veegcode is niet gevoelig voor de zaak, dus de "-" tekens zijn niet vereist.</span><span class="sxs-lookup"><span data-stu-id="80f11-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="80f11-111">Zie [Bypass-activeringsvergrendeling op iOS-apparaten met Intune voor](https://docs.microsoft.com/intune/device-activation-lock-bypass)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="80f11-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="80f11-112">**Veelgestelde vragen**</span><span class="sxs-lookup"><span data-stu-id="80f11-112">**FAQ**</span></span>

<span data-ttu-id="80f11-113">V: **Ik heb een actie op afstand uitgevaardigd om bedrijfsgegevens van een apparaat te verwijderen en nu zit deze vast in een in behandeling zijnde status.**</span><span class="sxs-lookup"><span data-stu-id="80f11-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="80f11-114">A: Om een actie op afstand succesvol te voltooien, moet het beoogde apparaat online en gezond zijn.</span><span class="sxs-lookup"><span data-stu-id="80f11-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="80f11-115">In de volgende situaties blijft de actie op afstand 30 dagen in behandeling of totdat het apparaat de opdracht erkent wanneer het apparaat:</span><span class="sxs-lookup"><span data-stu-id="80f11-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="80f11-116">Heeft geen connectiviteit.</span><span class="sxs-lookup"><span data-stu-id="80f11-116">Does not have connectivity.</span></span>
- <span data-ttu-id="80f11-117">Verliest zijn managementstatus bij Intune.</span><span class="sxs-lookup"><span data-stu-id="80f11-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="80f11-118">Als u denkt dat een apparaat niet meer incheckt en bedrijfsgegevens niet verwijdert, selecteert u Verwijderen.</span><span class="sxs-lookup"><span data-stu-id="80f11-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="80f11-119">Als u de apparaatrecord verwijdert, wordt de apparaatrecord verwijderd, zodat deze niet meer wordt weergegeven in de Intune-lijst met apparaten.</span><span class="sxs-lookup"><span data-stu-id="80f11-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="80f11-120">Als het apparaat weer actief wordt, moet de gebruiker het apparaat opnieuw inschrijven.</span><span class="sxs-lookup"><span data-stu-id="80f11-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="80f11-121">V: **Waarom zijn bepaalde acties op afstand niet beschikbaar voor mij om te gebruiken?**</span><span class="sxs-lookup"><span data-stu-id="80f11-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="80f11-122">A: Niet alle platforms ondersteunen alle acties op afstand.</span><span class="sxs-lookup"><span data-stu-id="80f11-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="80f11-123">De volgende acties op afstand zijn platformspecifiek.</span><span class="sxs-lookup"><span data-stu-id="80f11-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="80f11-124">Activeringsvergrendeling omzeilen (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="80f11-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="80f11-125">Nieuwe start (alleen Windows)</span><span class="sxs-lookup"><span data-stu-id="80f11-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="80f11-126">Verloren modus (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="80f11-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="80f11-127">Apparaat zoeken (alleen iOS)</span><span class="sxs-lookup"><span data-stu-id="80f11-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="80f11-128">Opnieuw opstarten (alleen Windows)</span><span class="sxs-lookup"><span data-stu-id="80f11-128">Restart (Windows only)</span></span>

<span data-ttu-id="80f11-129">Zie Acties voor beschikbare [apparaten](https://docs.microsoft.com/intune/device-management#available-device-actions)voor meer informatie over elke actie.</span><span class="sxs-lookup"><span data-stu-id="80f11-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>