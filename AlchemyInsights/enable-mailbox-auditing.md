---
title: Postvak-controle inschakelen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757813"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="b10ed-102">Postvak-controle inschakelen</span><span class="sxs-lookup"><span data-stu-id="b10ed-102">Enable mailbox auditing</span></span>

<span data-ttu-id="b10ed-103">Om een postbus controle inschakelen voor één gebruiker of een gehele organisatie moet de volgende cmdlets worden uitgevoerd vanuit externe Power Shell:</span><span class="sxs-lookup"><span data-stu-id="b10ed-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="b10ed-104">**Eén gebruiker**</span><span class="sxs-lookup"><span data-stu-id="b10ed-104">**Single User**</span></span>
  
<span data-ttu-id="b10ed-105">Set-Mailbox - identiteit "Jane Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="b10ed-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="b10ed-106">**Organisatie**</span><span class="sxs-lookup"><span data-stu-id="b10ed-106">**Organization**</span></span>
  
<span data-ttu-id="b10ed-107">Get-Mailbox - ResultSize onbeperkt - Filter {RecipientTypeDetails - eq "UserMailbox"} | $True set-Mailbox - AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="b10ed-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="b10ed-108">Meer informatie</span><span class="sxs-lookup"><span data-stu-id="b10ed-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

