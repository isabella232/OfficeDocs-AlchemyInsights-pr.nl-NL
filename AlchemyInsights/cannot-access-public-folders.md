---
title: Heeft geen toegang tot openbare mappen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891744"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="37d2d-102">Outlook kan geen verbinding maken met openbare mappen</span><span class="sxs-lookup"><span data-stu-id="37d2d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="37d2d-103">Als toegang tot openbare mappen voor sommige gebruikers niet werkt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="37d2d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="37d2d-104">Maak verbinding met EXO PowerShell en configureer de parameter DefaultPublicFolderMailbox op het probleemgebruikersaccount om de parameter op een werkend gebruikersaccount te matchen.</span><span class="sxs-lookup"><span data-stu-id="37d2d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="37d2d-105">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="37d2d-105">Example:</span></span>

<span data-ttu-id="37d2d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="37d2d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="37d2d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="37d2d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="37d2d-108">Wacht ten minste een uur tot de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="37d2d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="37d2d-109">Als het probleem blijft bestaan, volgt u [deze procedure](https://aka.ms/pfcte) om problemen met de toegang tot openbare mappen op te lossen met Outlook.</span><span class="sxs-lookup"><span data-stu-id="37d2d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>