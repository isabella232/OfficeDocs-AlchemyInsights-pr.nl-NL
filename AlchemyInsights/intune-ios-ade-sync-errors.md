---
title: Synchronisatiefouten met Apple-apparaten voor automatisch registreren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714738"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="71b0a-102">Synchronisatiefouten met Apple-apparaten voor automatisch registreren</span><span class="sxs-lookup"><span data-stu-id="71b0a-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="71b0a-103">' We hebben vastgesteld dat er een of meer ADE-of DEP-tokens zijn met een foutstatus.</span><span class="sxs-lookup"><span data-stu-id="71b0a-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="71b0a-104">Wanneer de foutstatus voor elk kwetsbaar token is opgelost, werkt de ADE-functionaliteit niet voor hetzelfde.</span><span class="sxs-lookup"><span data-stu-id="71b0a-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="71b0a-105">Deze fout kan op verschillende manieren worden weergegeven, zoals:</span><span class="sxs-lookup"><span data-stu-id="71b0a-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="71b0a-106">Apparaten worden mogelijk niet gesynchroniseerd van ABM/ASM naar intune</span><span class="sxs-lookup"><span data-stu-id="71b0a-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="71b0a-107">Toewijzing van registratie profielen is mogelijk mislukt</span><span class="sxs-lookup"><span data-stu-id="71b0a-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="71b0a-108">Mogelijk is de herregistratie van de hardware niet voltooid</span><span class="sxs-lookup"><span data-stu-id="71b0a-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="71b0a-109">Controleer of de synchronisatiefout is gerapporteerd in de intune-console onder **apparaten > schrijf apparatuur > Apple enrollment > tokens voor het registratieprogramma** en Raadpleeg de volgende documentatie voor een potentiële herstelactie:</span><span class="sxs-lookup"><span data-stu-id="71b0a-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="71b0a-110">Synchronisatiefouten in ABM/ASM voor iOS/iPadOS en macOS-registratie tokens voor automatisch apparaat</span><span class="sxs-lookup"><span data-stu-id="71b0a-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
