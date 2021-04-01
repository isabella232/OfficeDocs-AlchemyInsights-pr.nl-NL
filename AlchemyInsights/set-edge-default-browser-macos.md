---
title: Microsoft Edge instellen als de standaardbrowser op een macOS-apparaat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491425"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="4afd3-102">Microsoft Edge instellen als de standaardbrowser op een macOS-apparaat</span><span class="sxs-lookup"><span data-stu-id="4afd3-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="4afd3-103">Gebruik een van deze twee methoden om Microsoft Edge in te stellen als de standaardbrowser:</span><span class="sxs-lookup"><span data-stu-id="4afd3-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="4afd3-104">Methode 1: Knipper het apparaat met een afbeelding van macOS waarin Microsoft Edge al is ingesteld als de standaardbrowser.</span><span class="sxs-lookup"><span data-stu-id="4afd3-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="4afd3-105">Methode 2: Stel het beleid DefaultBrowserSettingEnabled in om de gebruiker te vragen Microsoft Edge in te stellen als de standaardbrowser.</span><span class="sxs-lookup"><span data-stu-id="4afd3-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="4afd3-106">Met beide methoden kan een gebruiker de standaardbrowser wijzigen.</span><span class="sxs-lookup"><span data-stu-id="4afd3-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="4afd3-107">Daarom wordt u aangeraden het beleid DefaultBrowserSettingEnabled te implementeren, zelfs als u methode 1 hebt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4afd3-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="4afd3-108">Als een gebruiker de standaardbrowser wijzigt nadat het beleid is geïmplementeerd, wordt de gebruiker gevraagd de standaardbrowser weer in te stellen op Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4afd3-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
