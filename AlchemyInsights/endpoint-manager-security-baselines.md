---
title: EndPoint Manager - Basislijnen voor beveiliging
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420775"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="9d7d4-102">EndPoint Manager - Basislijnen voor beveiliging</span><span class="sxs-lookup"><span data-stu-id="9d7d4-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="9d7d4-103">Beveiligingslijnlijnen zijn vooraf geconfigureerde groepen Windows-instellingen die u helpen bij het toepassen van de beveiligingsinstellingen die worden aanbevolen door de relevante beveiligingsteams.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="9d7d4-104">Deze basislijnen kunnen worden aangepast om alleen de gewenste instellingen en waarden te leveren.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="9d7d4-105">Zie Beveiligingslijnlijnen gebruiken om [Windows 10-apparaten in Intune te configureren voor meer informatie over beveiligingslijnlijnen.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="9d7d4-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="9d7d4-106">Er zijn momenteel basislijnen voor deze producten:</span><span class="sxs-lookup"><span data-stu-id="9d7d4-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="9d7d4-107">Windows MDM-beveiligingsinstellingen</span><span class="sxs-lookup"><span data-stu-id="9d7d4-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="9d7d4-108">Microsoft Defender voor EndPoint-beveiliging</span><span class="sxs-lookup"><span data-stu-id="9d7d4-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="9d7d4-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9d7d4-109">Microsoft Edge</span></span>

<span data-ttu-id="9d7d4-110">Elk van de basislijnen wordt regelmatig bijgewerkt en uitgebracht in incrementele versies.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="9d7d4-111">Met elke versie worden instellingen uit de vorige versie toegevoegd en of verwijderd om ervoor te zorgen dat de basislijn voldoet aan de huidige richtlijnen.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="9d7d4-112">Met de console Beveiligingslijnlijnen in Endpoint Security kunnen verschillende versies worden vergeleken door de wijzigingen van versie naar versie zichtbaar te maken.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="9d7d4-113">Zie Beveiligingslijnprofielen beheren [in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)voor informatie over het zo effectief mogelijk wijzigen van welke versie van basislijn wordt geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="9d7d4-114">Nadat u een beveiligingslijn hebt geïmplementeerd, kunt u de status van de implementatie controleren en de instellingen per apparaat controleren.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="9d7d4-115">**Opmerking:** Het kan maximaal 24 uur duren voordat de rapportagegegevens voor basislijnen worden weergegeven vanaf de eerste implementatie naar een apparaat en tot 6 uur voor verdere updates.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="9d7d4-116">De meest voorkomende oorzaak van het niet toepassen van een basislijninstelling is omdat dezelfde instelling wordt gebruikt in een ander profiel.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="9d7d4-117">Dit scenario kan worden onderzocht voor een specifiek apparaat door dat apparaat te selecteren in het knooppunt Apparaatstatus van het beveiligingslijnprofiel.</span><span class="sxs-lookup"><span data-stu-id="9d7d4-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="9d7d4-118">Zie Conflicten voor beveiligingslijnlijnen oplossen voor meer [informatie.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="9d7d4-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>