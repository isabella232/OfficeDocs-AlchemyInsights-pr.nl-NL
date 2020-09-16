---
title: Controle van Postvak inschakelen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806286"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="b1bc4-102">Controle van Postvak inschakelen</span><span class="sxs-lookup"><span data-stu-id="b1bc4-102">Enable mailbox auditing</span></span>

<span data-ttu-id="b1bc4-103">Als u controle van postvak wilt inschakelen voor één gebruiker of voor de hele organisatie, moeten de volgende cmdlets worden uitgevoerd vanaf een externe Power shell:</span><span class="sxs-lookup"><span data-stu-id="b1bc4-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="b1bc4-104">**Eén gebruiker**</span><span class="sxs-lookup"><span data-stu-id="b1bc4-104">**Single User**</span></span>
  
<span data-ttu-id="b1bc4-105">Set-mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="b1bc4-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="b1bc4-106">**Organisatie**</span><span class="sxs-lookup"><span data-stu-id="b1bc4-106">**Organization**</span></span>
  
<span data-ttu-id="b1bc4-107">Get-Mailbox-ResultSize Limited-filter {RecipientTypeDetails-EQ "User Mailbox"} | Set-mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="b1bc4-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="b1bc4-108">Meer informatie</span><span class="sxs-lookup"><span data-stu-id="b1bc4-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

