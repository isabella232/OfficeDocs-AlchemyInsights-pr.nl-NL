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
# <a name="11-call-recording"></a><span data-ttu-id="5d5c6-102">1:1-oproep opnemen</span><span class="sxs-lookup"><span data-stu-id="5d5c6-102">1:1 call recording</span></span>

<span data-ttu-id="5d5c6-103">Beheerders moeten nu actie ondernemen om ervoor te zorgen dat gebruikers 1:1-gesprekken kunnen opnemen.</span><span class="sxs-lookup"><span data-stu-id="5d5c6-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="5d5c6-104">Vanaf 12 april 2021 wordt een nieuwe optie voor het oproepbeleid van Teams *AllowCloudRecordingForCalls afdwingen.*</span><span class="sxs-lookup"><span data-stu-id="5d5c6-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="5d5c6-105">De mogelijkheden voor het opnemen van gesprekken met één op één worden momenteel bepaald door de *optie AllowCloudRecording* in Vergaderbeleid voor Teams.</span><span class="sxs-lookup"><span data-stu-id="5d5c6-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="5d5c6-106">Als uw gebruikers toestemming hebben om Teams-vergaderingen op te nemen, kunnen ze ook een-op-een-gesprekken opnemen.</span><span class="sxs-lookup"><span data-stu-id="5d5c6-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="5d5c6-107">Als u liever niet wilt dat alle gebruikers een-op-een-gesprekken kunnen opnemen, hoeft u niets te doen.</span><span class="sxs-lookup"><span data-stu-id="5d5c6-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="5d5c6-108">*De beleidsoptie AllowCloudRecordingForCalls* wordt $False standaard uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5d5c6-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="5d5c6-109">Deze wijziging wordt beschreven in het volgende bericht in het berichtencentrum: [(Bijgewerkt) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introductie tot oproepopnamebeleid Om de optie Oproepbeleid voor Teams in te stellen, moet u [Teams PowerShell gebruiken.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="5d5c6-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="5d5c6-110">**Oproepopname inschakelen in een-op-een-gesprekken:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="5d5c6-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="5d5c6-111">**Oproepopname uitschakelen in een-op-een-gesprekken:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="5d5c6-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

