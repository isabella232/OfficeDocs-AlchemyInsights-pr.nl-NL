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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostisch hulpprogramma voor Windows virtueel bureaublad

Windows virtueel bureaublad (WVD) biedt een diagnostisch hulpprogramma waarmee beheerders fouten kunnen identificeren via één interface. Met dit hulpprogramma worden diagnostische gegevens vastgelegd wanneer WVD wordt gebruikt door iemand die een WVD-rol heeft toegewezen. Elk logboek bevat informatie over de WVD-rol bij de activiteit, de foutberichten die tijdens de sessie worden weergegeven en de informatie over de Tenant en de gebruiker. Azure log Analytics kan worden geconfigureerd voor het vastleggen van het activiteitenlogboek dat door het diagnostisch hulpprogramma is gemaakt. Hier ziet u hoe dat gaat:

1. Maak een werkruimte voor logboekanalyse met de [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) of [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Windows-computers verbinden met Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Zorg dat de ID van de werkruimte en de primaire sleutel van de werkruimte zijn. De installatiewizard heeft deze gegevens nodig om de agent correct te configureren en om ervoor te zorgen dat deze kan communiceren met Azure monitor.
1. [Diagnostische gegevens naar uw werkruimte duwen](https://go.microsoft.com/fwlink/?linkid=2128284) U kunt Diagnostische gegevens van uw WVD-Tenant naar de logboekanalyse voor uw werkruimte pushen.
1. [Identificeer en diagnose problemen](https://go.microsoft.com/fwlink/?linkid=2128338) die intern of extern zijn in verband met WVD.

Zie [logboekanalyse gebruiken voor de diagnostische functie](https://go.microsoft.com/fwlink/?linkid=2128084)voor meer informatie over het configureren van het hulpprogramma servicecontrole voor WVD.
