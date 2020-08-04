---
title: Automatisch opruimen van verouderde apparaten in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554964"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="f3d65-102">Automatisch opruimen van verouderde apparaten in Intune</span><span class="sxs-lookup"><span data-stu-id="f3d65-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="f3d65-103">Intune stelt de beheerder in staat om een tijdsinterval tussen 90 en 270 dagen te configureren, waarna verouderde apparaten uit de service worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="f3d65-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="f3d65-104">Deze instelling is organisatiebreed en zodra geactiveerd gaat onmiddellijk in werking.</span><span class="sxs-lookup"><span data-stu-id="f3d65-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="f3d65-105">Apparaten die gedurende een periode die de instelling overschrijdt, niet in de Intune-server zijn ingecheckt, worden permanent verwijderd.</span><span class="sxs-lookup"><span data-stu-id="f3d65-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="f3d65-106">**Opmerking** Alleen MDM-apparaatobjecten komen in aanmerking voor deze opruimactie.</span><span class="sxs-lookup"><span data-stu-id="f3d65-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="f3d65-107">EAS-apparaatobjecten zijn uitgesloten.</span><span class="sxs-lookup"><span data-stu-id="f3d65-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="f3d65-108">Voor aanvullende informatie over wanneer een apparaat in aanmerking komt voor verwijdering op basis van de installatie van het apparaat en de "status":</span><span class="sxs-lookup"><span data-stu-id="f3d65-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="f3d65-109">Instelling: **Apparaten verwijderen na laatste incheckdatum: Ja (enkele waarde (N) in opgegeven dagen)**</span><span class="sxs-lookup"><span data-stu-id="f3d65-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="f3d65-110">Op basis van de in de instelling geconfigureerde waarde (N) verwijdert de Intune-service het apparaat in de opgegeven dagen nadat het laatste met succes is ingecheckt.</span><span class="sxs-lookup"><span data-stu-id="f3d65-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="f3d65-111">Instelling: **Apparaten verwijderen na laatste incheckdatum: Nee**</span><span class="sxs-lookup"><span data-stu-id="f3d65-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="f3d65-112">180 dagen nadat het apparaatcertificaat is verlopen en niet wordt verlengd, wordt het apparaat verwijderd.</span><span class="sxs-lookup"><span data-stu-id="f3d65-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="f3d65-113">**Opmerking** In beide gevallen moet het apparaat met succes worden geregistreerd in Intune.</span><span class="sxs-lookup"><span data-stu-id="f3d65-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="f3d65-114">Registratie vindt plaats tijdens het eerste apparaat inchecken met de Intune-service.</span><span class="sxs-lookup"><span data-stu-id="f3d65-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="f3d65-115">Als een apparaat zich met succes inschrijft voor Intune maar niet intune wordt geregistreerd, wordt het apparaat 270 dagen na inschrijving verwijderd.</span><span class="sxs-lookup"><span data-stu-id="f3d65-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="f3d65-116">(90 dagen om het apparaat als ingetrokken te markeren en vervolgens nog eens 180 dagen om de record te verwijderen.)</span><span class="sxs-lookup"><span data-stu-id="f3d65-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="f3d65-117">Er bestaat momenteel geen mechanisme in de Intune-console om de vervaldatum van de apparaatcertificering voor een bepaald apparaat vast te stellen.</span><span class="sxs-lookup"><span data-stu-id="f3d65-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>