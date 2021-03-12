---
title: 1:1-oproep opnemen
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733844"
---
# <a name="11-call-recording"></a>1:1-oproep opnemen

Beheerders moeten nu actie ondernemen om ervoor te zorgen dat gebruikers 1:1-gesprekken kunnen opnemen.
 
Vanaf 12 april 2021 wordt een nieuwe optie voor het oproepbeleid van Teams *AllowCloudRecordingForCalls afdwingen.* 

De mogelijkheden voor het opnemen van gesprekken met één op één worden momenteel bepaald door de *optie AllowCloudRecording* in Vergaderbeleid voor Teams. Als uw gebruikers toestemming hebben om Teams-vergaderingen op te nemen, kunnen ze ook een-op-een-gesprekken opnemen.

Als u liever niet wilt dat alle gebruikers een-op-een-gesprekken kunnen opnemen, hoeft u niets te doen. *De beleidsoptie AllowCloudRecordingForCalls* wordt $False standaard uitgeschakeld.

Deze wijziging wordt beschreven in het volgende bericht in het berichtencentrum: [(Bijgewerkt) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introductie tot oproepopnamebeleid Om de optie Oproepbeleid voor Teams in te stellen, moet u [Teams PowerShell gebruiken.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Oproepopname inschakelen in een-op-een-gesprekken:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Oproepopname uitschakelen in een-op-een-gesprekken:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

