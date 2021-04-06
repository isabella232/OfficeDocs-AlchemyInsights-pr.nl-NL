---
title: Hulpprogramma voor servicediagnose voor Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595633"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="a4129-102">Hulpprogramma voor servicediagnose voor Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="a4129-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="a4129-103">Windows Virtual Desktop (WVD) biedt een diagnostisch hulpprogramma waarmee beheerders fouten kunnen identificeren via één interface.</span><span class="sxs-lookup"><span data-stu-id="a4129-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="a4129-104">Dit hulpprogramma registreert diagnostische gegevens wanneer WVD wordt gebruikt door iemand die een WVD-rol heeft toegewezen.</span><span class="sxs-lookup"><span data-stu-id="a4129-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="a4129-105">Elk logboek bevat informatie over de WVD-rol die betrokken is bij de activiteit, de foutberichten die tijdens de sessie worden weergegeven en de informatie over de tenant en de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="a4129-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="a4129-106">Azure Log Analytics kan worden geconfigureerd om het activiteitenlogboek vast te leggen dat door het diagnostische hulpprogramma is gemaakt door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="a4129-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="a4129-107">Maak een loganalysewerkruimte met de [Azure-portal](https://go.microsoft.com/fwlink/?linkid=2129500) of [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="a4129-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="a4129-108">[Sluit Windows-computers aan op Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="a4129-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="a4129-109">Haal de werkruimte-id en de primaire sleutel van uw werkruimte op.</span><span class="sxs-lookup"><span data-stu-id="a4129-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="a4129-110">De installatiewizard heeft deze gegevens nodig om de agent correct te configureren en ervoor te zorgen dat deze kan communiceren met Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="a4129-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="a4129-111">[Diagnostische gegevens naar uw werkruimte pushen.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="a4129-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="a4129-112">U kunt diagnostische gegevens van uw WVD-tenant naar loganalyse voor uw werkruimte pushen.</span><span class="sxs-lookup"><span data-stu-id="a4129-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="a4129-113">[Identificeer en diagnosticer](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemen die intern of extern zijn met betrekking tot WVD.</span><span class="sxs-lookup"><span data-stu-id="a4129-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="a4129-114">Zie Loganalyse gebruiken voor de diagnostische functie voor meer informatie over het configureren van het hulpprogramma voor servicediagnose voor WVD.</span><span class="sxs-lookup"><span data-stu-id="a4129-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>