---
title: Problemen met Windows Virtual Desktop identificeren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595626"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="fc6a1-102">Problemen met Windows Virtual Desktop identificeren</span><span class="sxs-lookup"><span data-stu-id="fc6a1-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="fc6a1-103">Windows Virtual Desktop Diagnostics gebruikt slechts één PowerShell-cmdlet, maar bevat veel optionele parameters om problemen te beperken en te isoleren.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="fc6a1-104">Aan de slag:</span><span class="sxs-lookup"><span data-stu-id="fc6a1-104">To get started:</span></span> 

1. <span data-ttu-id="fc6a1-105">Download en importeer de Windows Virtual Desktop PowerShell-module.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="fc6a1-106">Zie Windows [Virtual Desktop Cmdlets voor Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="fc6a1-107">Voer de volgende cmdlet uit om u aan te melden bij uw account:</span><span class="sxs-lookup"><span data-stu-id="fc6a1-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="fc6a1-108">Voorbeeld: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="fc6a1-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="fc6a1-109">**OPMERKING:** Alle query's die PowerShell gebruiken, moeten de parameters -UserName of -ActivityID bevatten.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="fc6a1-110">Zie Logboekanalyse gebruiken voor de [functie diagnostische functies](https://go.microsoft.com/fwlink/?linkid=2126847)voor het controleren van mogelijkheden.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="fc6a1-111">Als u diagnostische activiteiten wilt filteren op gebruiker, moet u de volgende cmdlet uitvoeren:</span><span class="sxs-lookup"><span data-stu-id="fc6a1-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="fc6a1-112">Voorbeeld: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="fc6a1-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="fc6a1-113">Er is een lijst met filters die u kunt uitvoeren om problemen te diagnosticeren.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="fc6a1-114">Zie Problemen met Windows Virtual Desktop identificeren en diagnosticeren voor meer informatie over het diagnosticeren van [problemen.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="fc6a1-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="fc6a1-115">Zie Veelvoorkomende fouten [senario's](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)voor meer informatie over veelvoorkomende fouten.</span><span class="sxs-lookup"><span data-stu-id="fc6a1-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
