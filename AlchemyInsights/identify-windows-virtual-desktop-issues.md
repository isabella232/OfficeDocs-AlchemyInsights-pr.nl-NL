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
# <a name="identify-windows-virtual-desktop-issues"></a>Problemen met Windows Virtual Desktop identificeren

Windows Virtual Desktop Diagnostics gebruikt slechts één PowerShell-cmdlet, maar bevat veel optionele parameters om problemen te beperken en te isoleren. Aan de slag: 

1. Download en importeer de Windows Virtual Desktop PowerShell-module. Zie Windows [Virtual Desktop Cmdlets voor Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)voor meer informatie.

1. Voer de volgende cmdlet uit om u aan te melden bij uw account:
    
    Voorbeeld: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**OPMERKING:** Alle query's die PowerShell gebruiken, moeten de parameters -UserName of -ActivityID bevatten. Zie Logboekanalyse gebruiken voor de [functie diagnostische functies](https://go.microsoft.com/fwlink/?linkid=2126847)voor het controleren van mogelijkheden.

Als u diagnostische activiteiten wilt filteren op gebruiker, moet u de volgende cmdlet uitvoeren:

Voorbeeld: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Er is een lijst met filters die u kunt uitvoeren om problemen te diagnosticeren. Zie Problemen met Windows Virtual Desktop identificeren en diagnosticeren voor meer informatie over het diagnosticeren van [problemen.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Zie Veelvoorkomende fouten [senario's](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)voor meer informatie over veelvoorkomende fouten.
