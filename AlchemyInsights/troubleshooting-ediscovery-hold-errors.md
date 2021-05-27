---
title: Problemen met ediscovery oplossen bevat fouten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676085"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="e1e91-102">Problemen met ediscovery oplossen bevat fouten</span><span class="sxs-lookup"><span data-stu-id="e1e91-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="e1e91-103">Ondervindt u problemen met eDiscovery-bezit?</span><span class="sxs-lookup"><span data-stu-id="e1e91-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="e1e91-104">Hier volgen enkele best practices om rekening mee te houden:</span><span class="sxs-lookup"><span data-stu-id="e1e91-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="e1e91-105">Controleer de distributiestatus van de wacht.</span><span class="sxs-lookup"><span data-stu-id="e1e91-105">Check the hold distribution status.</span></span>  <span data-ttu-id="e1e91-106">Als de status **Aan (In behandeling)** of **Uit (In behandeling)** is, wacht u totdat de distributie in de wacht is gezet.</span><span class="sxs-lookup"><span data-stu-id="e1e91-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="e1e91-107">EDiscovery-holdupdates samenvoegen in één bulkaanvraag in plaats van het beleid herhaaldelijk bij te werken voor elke transactie.</span><span class="sxs-lookup"><span data-stu-id="e1e91-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="e1e91-108">Voer Set-CaseHoldPolicy <policyname> -RetryDistribution uit in het Powershell-beveiligings- en compliancecentrum.</span><span class="sxs-lookup"><span data-stu-id="e1e91-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="e1e91-109">Zie Verbinding maken & PowerShell voor [meer informatie.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="e1e91-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="e1e91-110">Zie Problemen met eDiscovery oplossen voor stappen om deze instellingen en aanvullende best practices voor het voorkomen en oplossen van problemen met [eDiscovery te controleren.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="e1e91-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="e1e91-111">Zie Veelvoorkomende eDiscovery-problemen onderzoeken, oplossen en oplossen voor informatie over het oplossen van andere veelvoorkomende [eDiscovery-problemen.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="e1e91-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
