---
title: Service diagnostisch hulpprogramma voor Windows virtueel bureaublad
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677650"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="f5f0d-102">Service diagnostisch hulpprogramma voor Windows virtueel bureaublad</span><span class="sxs-lookup"><span data-stu-id="f5f0d-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="f5f0d-103">Windows virtueel bureaublad (WVD) biedt een diagnostisch hulpprogramma waarmee beheerders fouten kunnen identificeren via één interface.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="f5f0d-104">Met dit hulpprogramma worden diagnostische gegevens vastgelegd wanneer WVD wordt gebruikt door iemand die een WVD-rol heeft toegewezen.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="f5f0d-105">Elk logboek bevat informatie over de WVD-rol bij de activiteit, de foutberichten die tijdens de sessie worden weergegeven en de informatie over de Tenant en de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="f5f0d-106">Azure log Analytics kan worden geconfigureerd voor het vastleggen van het activiteitenlogboek dat door het diagnostisch hulpprogramma is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="f5f0d-107">Hier ziet u hoe dat gaat:</span><span class="sxs-lookup"><span data-stu-id="f5f0d-107">Here's how:</span></span>

1. <span data-ttu-id="f5f0d-108">Maak een werkruimte voor logboekanalyse met de [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) of [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="f5f0d-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="f5f0d-109">[Windows-computers verbinden met Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="f5f0d-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="f5f0d-110">Zorg dat de ID van de werkruimte en de primaire sleutel van de werkruimte zijn.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="f5f0d-111">De installatiewizard heeft deze gegevens nodig om de agent correct te configureren en om ervoor te zorgen dat deze kan communiceren met Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="f5f0d-112">[Diagnostische gegevens naar uw werkruimte duwen](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="f5f0d-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="f5f0d-113">U kunt Diagnostische gegevens van uw WVD-Tenant naar de logboekanalyse voor uw werkruimte pushen.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="f5f0d-114">[Identificeer en diagnose problemen](https://go.microsoft.com/fwlink/?linkid=2128338) die intern of extern zijn in verband met WVD.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="f5f0d-115">Zie [logboekanalyse gebruiken voor de diagnostische functie](https://go.microsoft.com/fwlink/?linkid=2128084)voor meer informatie over het configureren van het hulpprogramma servicecontrole voor WVD.</span><span class="sxs-lookup"><span data-stu-id="f5f0d-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
