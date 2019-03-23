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
# <a name="enable-mailbox-auditing"></a>Postvak-controle inschakelen

Om een postbus controle inschakelen voor één gebruiker of een gehele organisatie moet de volgende cmdlets worden uitgevoerd vanuit externe Power Shell:
  
 **Eén gebruiker**
  
Set-Mailbox - identiteit "Jane Dow" - AuditEnabled $true
  
 **Organisatie**
  
Get-Mailbox - ResultSize onbeperkt - Filter {RecipientTypeDetails - eq "UserMailbox"} | $True set-Mailbox - AuditEnabled
  
[Meer informatie](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

