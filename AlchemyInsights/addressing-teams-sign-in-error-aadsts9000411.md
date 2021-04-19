---
title: Aanmeldingsfout voor Teams aanpakken AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821982"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="9ca40-102">Aanmeldingsfout voor Teams aanpakken AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="9ca40-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="9ca40-103">Wanneer u zich aanmeldt bij Microsoft Teams, krijgt u mogelijk de foutmelding: Sorry, maar we hebben problemen met het ondertekenen van u **in AADSTS9000411: De aanvraag is niet correct opgemaakt. De parameter 'login_hint' wordt gedupliceerd.**</span><span class="sxs-lookup"><span data-stu-id="9ca40-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="9ca40-104">Als u dit probleem wilt oplossen, moet u ervoor zorgen dat uw Microsoft Teams-clients worden bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="9ca40-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="9ca40-105">Zie Microsoft Teams bijwerken voor meer informatie over het bijwerken [van uw client.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="9ca40-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="9ca40-106">Als u uw client om wat voor reden dan ook niet kunt bijwerken, worden de meeste gegevens in de cache verwijderd als u zich afmeldt bij de client.</span><span class="sxs-lookup"><span data-stu-id="9ca40-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="9ca40-107">Als u echter nog steeds problemen hebt na het logoff/aanmelding, sluit u Teams af en leegt u de cache van uw client door het volgende te doen:</span><span class="sxs-lookup"><span data-stu-id="9ca40-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="9ca40-108">Sluit Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9ca40-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="9ca40-109">Ga naar: %appdata%\microsoft\teams en verwijder alle bestanden.</span><span class="sxs-lookup"><span data-stu-id="9ca40-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="9ca40-110">Open Microsoft Teams opnieuw.</span><span class="sxs-lookup"><span data-stu-id="9ca40-110">Reopen Microsoft Teams.</span></span>
