---
title: Regels voor het verminderen van kwetsbaarheid voor aanvallen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676127"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="29516-102">Regels voor het verminderen van kwetsbaarheid voor aanvallen</span><span class="sxs-lookup"><span data-stu-id="29516-102">Attack surface reduction rules</span></span>

<span data-ttu-id="29516-103">Het uitsluiten van bestanden of mappen kan de beveiliging die wordt geboden door regels voor het beperken van het oppervlak van de aanval, aanzienlijk beperken.</span><span class="sxs-lookup"><span data-stu-id="29516-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="29516-104">Bestanden die door een regel zijn geblokkeerd, mogen worden uitgevoerd en er wordt geen rapport of gebeurtenis opgenomen.</span><span class="sxs-lookup"><span data-stu-id="29516-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="29516-105">Een uitsluiting is van toepassing op alle regels die uitsluitingen toestaan.</span><span class="sxs-lookup"><span data-stu-id="29516-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="29516-106">Asr-uitsluitingen gebruiken dezelfde syntaxis als Microsoft Defender Antivirus uitsluitingen.</span><span class="sxs-lookup"><span data-stu-id="29516-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="29516-107">Zie Uitsluitingen [configureren en valideren voor](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)Microsoft Defender Antivirus scans voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="29516-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="29516-108">Als u problemen wilt voorkomen, bekijkt u [Veelvoorkomende fouten om te voorkomen bij het definiëren van uitsluitingen.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="29516-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="29516-109">Niet alle ASR-regels ondersteunen uitsluitingen.</span><span class="sxs-lookup"><span data-stu-id="29516-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="29516-110">Als u wilt valideren of uw regel uitsluitingen ondersteunt, bekijkt u de tabel [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="29516-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="29516-111">Regels voor het verminderen van kwetsbaarheid voor aanvallen</span><span class="sxs-lookup"><span data-stu-id="29516-111">Attack surface reduction rules</span></span>

<span data-ttu-id="29516-112">De surface van uw organisatie-aanval bevat alle locaties waar een aanvaller organisatieapparaten of netwerken kan compromitteerden.</span><span class="sxs-lookup"><span data-stu-id="29516-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="29516-113">Als u uw aanvalsoppervlak verkleint, moet u de organisatieapparaten en het netwerk beschermen, waardoor aanvallers minder manieren hebben om aanvallen uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="29516-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="29516-114">Het configureren van regels voor het verlagen van de Surface-aanval in Microsoft Defender voor Eindpunt kan u helpen.</span><span class="sxs-lookup"><span data-stu-id="29516-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="29516-115">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="29516-115">For more information, see:</span></span>

- [<span data-ttu-id="29516-116">ASR-regel GUID aan een naam geven</span><span class="sxs-lookup"><span data-stu-id="29516-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="29516-117">VEREISTEN VOOR ASR-regels:</span><span class="sxs-lookup"><span data-stu-id="29516-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="29516-118">Windows 10 Pro, versie 1709 of hoger</span><span class="sxs-lookup"><span data-stu-id="29516-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="29516-119">Windows 10 Enterprise, versie 1709 of hoger</span><span class="sxs-lookup"><span data-stu-id="29516-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="29516-120">Windows Server, versie 1803 (halfjaarlijks kanaal) of hoger</span><span class="sxs-lookup"><span data-stu-id="29516-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="29516-121">De juiste uitsluiting identificeren die moet worden toegepast</span><span class="sxs-lookup"><span data-stu-id="29516-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="29516-122">Zoek naar eventID 1121 of 1122 in het Microsoft-Windows-Windows Defender/Operational log.</span><span class="sxs-lookup"><span data-stu-id="29516-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="29516-123">Evalueer het blokscenario en de context en bevestig dat dit scenario moet worden geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="29516-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="29516-124">Lees de waarde Pad in de gebeurtenisdetails, de waarde die de uitsluiting definieert.</span><span class="sxs-lookup"><span data-stu-id="29516-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="29516-125">Maak de uitsluiting zo strikt mogelijk.</span><span class="sxs-lookup"><span data-stu-id="29516-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="29516-126">Pas indien nodig een jokerteken toe (vervang bijvoorbeeld de variabele Gebruiker).</span><span class="sxs-lookup"><span data-stu-id="29516-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="29516-127">Pas de uitsluiting toe op basis van uw implementatiebehoeften.</span><span class="sxs-lookup"><span data-stu-id="29516-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="29516-128">Zie Attack [Surface Reduction Rules aanpassen voor meer informatie.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="29516-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="29516-129">Uitsluiting wordt niet nagekomen</span><span class="sxs-lookup"><span data-stu-id="29516-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="29516-130">Bepaal of de regel uitsluitingen ondersteunt.</span><span class="sxs-lookup"><span data-stu-id="29516-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="29516-131">Zie Surface [Reduction Rules attack (Surface Reduction Rules) voor meer informatie.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="29516-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="29516-132">Controleer de toegepaste uitsluitingen en controleer met de gebeurtenisgegevens op typefouten of onjuist geïnterpreteerde jokertekens.</span><span class="sxs-lookup"><span data-stu-id="29516-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="29516-133">Zie Ondersteunde [uitsluitingstypen voor meer informatie](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="29516-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="29516-134">als de invloed van de regel te hoog is, kunt u overwegen de regel (terug) te verplaatsen naar de auditmodus om verdere validatie uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="29516-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="29516-135">Zie Testen hoe Microsoft Defender voor eindpuntfuncties werken [in de auditmodus](/microsoft-365/security/defender-endpoint/audit-windows-defender)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="29516-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="29516-136">Verzamel ondersteuningsgegevens om een ondersteuningscase te openen met behulp van deze opdracht:</span><span class="sxs-lookup"><span data-stu-id="29516-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="29516-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="29516-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="29516-138">Zie Problemen met [onboarding-machines](issues-with-onboarding-machines.md)bij Microsoft Defender voor eindpunten voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="29516-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
