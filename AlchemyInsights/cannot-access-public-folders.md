---
title: Geen toegang tot openbare mappen
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959490"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="94535-102">Outlook kan geen verbinding maken met openbare mappen</span><span class="sxs-lookup"><span data-stu-id="94535-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="94535-103">Als de toegang tot openbare mappen niet voor enkele gebruikers werkt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="94535-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="94535-104">Maak verbinding met EXO PowerShell en configureer de DefaultPublicFolderMailbox op het probleem gebruikersaccount zodat deze overeenkomt met een in een werkend gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="94535-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="94535-105">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="94535-105">Example:</span></span>

<span data-ttu-id="94535-106">Get-Mailbox Workinggebruiker | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="94535-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="94535-107">Set-mailbox ProblemUser-DefaultPublicFolderMailbox \<waarde van de vorige opdracht></span><span class="sxs-lookup"><span data-stu-id="94535-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="94535-108">Wacht ten minste één uur voordat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="94535-108">Wait at least one hour for the change to take effect.</span></span>