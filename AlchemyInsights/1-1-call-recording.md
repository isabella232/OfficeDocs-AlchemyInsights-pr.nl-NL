---
title: 1:1 oproepopname
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702085"
---
# <a name="11-call-recording"></a>1:1 oproepopname

Als de **knop Opname** starten grijs wordt weergegeven in een 1:1-gesprek, moet u de beleidsinstellingen voor de beïnvloede gebruiker wijzigen. Als u de beleidsinstelling wilt controleren, kunt u de diagnostische instelling voor de beïnvloede gebruiker uitvoeren door **Diag: Teams 1:1 Gespreksopname** hierboven te typen.     

Vanaf 31 mei 2021 gaan we een nieuwe Teams Belbeleid *AllowCloudRecordingForCalls afdwingen.* Vóór deze wijziging wordt de opname van 1:1-gesprekken bepaald door *het Teams AllowCloudRecording.* Deze wijziging wordt beschreven in het Berichtcentrumbericht: [(Bijgewerkt) 1:1 Beleidsintroductie voor het](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)opnemen van gesprekken.  

*AllowCloudRecordingForCalls*   De optie voor het bellen van het **$False** standaard ingesteld. Als u wilt blokkeren dat alle gebruikers 1:1-oproepen opnemen, hoeft u geen actie te ondernemen.  

Als u oproepopname wilt inschakelen voor alle gebruikers in 1:1-oproepen, gebruikt [u Teams PowerShell](/microsoftteams/teams-powershell-install) om de volgende cmdlet uit te voeren: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

U kunt ook een nieuw beleid maken en **AllowCloudRecordingForCalls** instellen voor $true **en** dat beleid toewijzen aan uw gebruikers. 

Zie [1:1 Gespreksopnamebeleidsbesturingselementen zijn (bijna!) voor meer informatie. Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
