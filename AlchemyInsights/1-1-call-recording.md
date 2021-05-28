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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696917"
---
# <a name="11-call-recording"></a><span data-ttu-id="f9236-102">1:1 oproepopname</span><span class="sxs-lookup"><span data-stu-id="f9236-102">1:1 call recording</span></span>

<span data-ttu-id="f9236-103">Als de **knop Opname** starten grijs wordt weergegeven in een 1:1-gesprek, moet u de beleidsinstellingen voor de beïnvloede gebruiker wijzigen.</span><span class="sxs-lookup"><span data-stu-id="f9236-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="f9236-104">Vanaf 31 mei 2021 gaan we een nieuwe Teams Belbeleid *AllowCloudRecordingForCalls afdwingen.*</span><span class="sxs-lookup"><span data-stu-id="f9236-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="f9236-105">Vóór deze wijziging wordt de opname van 1:1-gesprekken bepaald door *het Teams AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="f9236-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="f9236-106">Deze wijziging wordt beschreven in het Berichtcentrumbericht: [(Bijgewerkt) 1:1 Beleidsintroductie voor het](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)opnemen van gesprekken.</span><span class="sxs-lookup"><span data-stu-id="f9236-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="f9236-107">*AllowCloudRecordingForCalls*   De optie voor het bellen van het **$False** standaard ingesteld.</span><span class="sxs-lookup"><span data-stu-id="f9236-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="f9236-108">Als u wilt blokkeren dat alle gebruikers 1:1-oproepen opnemen, hoeft u geen actie te ondernemen.</span><span class="sxs-lookup"><span data-stu-id="f9236-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="f9236-109">Als u oproepopname wilt inschakelen voor alle gebruikers in 1:1-oproepen, gebruikt u Teams PowerShell om de volgende cmdlet uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="f9236-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="f9236-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="f9236-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="f9236-111">U kunt ook een nieuw beleid maken en **AllowCloudRecordingForCalls** instellen voor $true **en** dat beleid toewijzen aan uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="f9236-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="f9236-112">Zie [1:1 Gespreksopnamebeleidsbesturingselementen zijn (bijna!) voor meer informatie. Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="f9236-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
