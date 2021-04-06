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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Hulpprogramma voor servicediagnose voor Windows Virtual Desktop

Windows Virtual Desktop (WVD) biedt een diagnostisch hulpprogramma waarmee beheerders fouten kunnen identificeren via één interface. Dit hulpprogramma registreert diagnostische gegevens wanneer WVD wordt gebruikt door iemand die een WVD-rol heeft toegewezen. Elk logboek bevat informatie over de WVD-rol die betrokken is bij de activiteit, de foutberichten die tijdens de sessie worden weergegeven en de informatie over de tenant en de gebruiker. Azure Log Analytics kan worden geconfigureerd om het activiteitenlogboek vast te leggen dat door het diagnostische hulpprogramma is gemaakt door de volgende stappen uit te voeren:

1. Maak een loganalysewerkruimte met de [Azure-portal](https://go.microsoft.com/fwlink/?linkid=2129500) of [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Sluit Windows-computers aan op Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Haal de werkruimte-id en de primaire sleutel van uw werkruimte op. De installatiewizard heeft deze gegevens nodig om de agent correct te configureren en ervoor te zorgen dat deze kan communiceren met Azure Monitor.

1. [Diagnostische gegevens naar uw werkruimte pushen.](https://go.microsoft.com/fwlink/?linkid=2128284) U kunt diagnostische gegevens van uw WVD-tenant naar loganalyse voor uw werkruimte pushen.

1. [Identificeer en diagnosticer](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemen die intern of extern zijn met betrekking tot WVD.

Zie Loganalyse gebruiken voor de diagnostische functie voor meer informatie over het configureren van het hulpprogramma voor servicediagnose voor WVD.