---
title: EndPoint Manager - beveiligingsbasislijnen
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440876"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="0daed-102">EndPoint Manager - beveiligingsbasislijnen</span><span class="sxs-lookup"><span data-stu-id="0daed-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="0daed-103">Beveiligingsbasislijnen zijn vooraf geconfigureerde groepen Windows-instellingen die u helpen bij het toepassen van de beveiligingsinstellingen die door de relevante beveiligingsteams worden aanbevolen.</span><span class="sxs-lookup"><span data-stu-id="0daed-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="0daed-104">U kunt deze basislijnen aanpassen om alleen de instellingen en waarden te kunnen leveren.</span><span class="sxs-lookup"><span data-stu-id="0daed-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="0daed-105">Voor meer informatie over beveiligingsbasislijnen, zie [Beveiligingsbasislijnen gebruiken om Windows 10-apparaten te configureren in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="0daed-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="0daed-106">Er zijn momenteel basislijnen voor deze producten:</span><span class="sxs-lookup"><span data-stu-id="0daed-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="0daed-107">Windows MDM-beveiligingsinstellingen</span><span class="sxs-lookup"><span data-stu-id="0daed-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="0daed-108">Microsoft Defender voor eindpuntbeveiliging</span><span class="sxs-lookup"><span data-stu-id="0daed-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="0daed-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0daed-109">Microsoft Edge</span></span>

<span data-ttu-id="0daed-110">Alle basislijnen wordt periodiek bijgewerkt en uitgebracht in incrementele versies.</span><span class="sxs-lookup"><span data-stu-id="0daed-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="0daed-111">In elke versie worden instellingen toegevoegd en verwijderd uit de vorige versie om ervoor te zorgen dat de basislijn voldoet aan de huidige richtlijnen.</span><span class="sxs-lookup"><span data-stu-id="0daed-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="0daed-112">Met de console voor beveiligingsbasislijnen in Eindpuntbeveiliging, kunnen verschillende versies worden vergeleken door de wijzigingen van versie naar versie zichtbaar te maken.</span><span class="sxs-lookup"><span data-stu-id="0daed-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="0daed-113">Voor instructies om zo effectief mogelijk te wijzigen welke basislijnversie is geïmplementeerd, zie [Profielen voor beveiligingsbasislijn beheren in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="0daed-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="0daed-114">Nadat u een basislijn voor beveiliging hebt geïmplementeerd, kunt u de status van de implementatie controleren en de instellingen per apparaat controleren.</span><span class="sxs-lookup"><span data-stu-id="0daed-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="0daed-115">**Opmerking:** Het kan maximaal 24 uur duren voordat de rapportagegegevens voor basislijnen worden weergegeven vanaf de eerste implementatie op een apparaat en tot 6 uur voor verdere updates.</span><span class="sxs-lookup"><span data-stu-id="0daed-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="0daed-116">De meest voorkomende oorzaak voor het niet-toepassen van een basislijninstelling is dat dezelfde instelling in een ander profiel wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="0daed-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="0daed-117">U kunt dit scenario onderzoeken op een specifiek apparaat door dat apparaat te selecteren in het knooppunt Apparaatstatus van het profiel Beveiligingsbasislijnen.</span><span class="sxs-lookup"><span data-stu-id="0daed-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="0daed-118">Voor meer informatie, zie [Conflicten in beveiligingsbasislijnen oplossen](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="0daed-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>