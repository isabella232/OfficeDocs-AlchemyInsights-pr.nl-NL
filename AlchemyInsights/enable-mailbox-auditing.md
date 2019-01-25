---
title: Postvak-controle inschakelen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500277"
---
# <a name="enable-mailbox-auditing"></a>Postvak-controle inschakelen

Om een postbus controle inschakelen voor één gebruiker of een gehele organisatie moet de volgende cmdlets worden uitgevoerd vanuit externe Power Shell:
  
 **Eén gebruiker**
  
Set-Mailbox - identiteit "Jane Dow" - AuditEnabled $true
  
 **Organisatie**
  
Get-Mailbox - ResultSize onbeperkt - Filter {RecipientTypeDetails - eq "UserMailbox"} | $True set-Mailbox - AuditEnabled
  
[Meer informatie](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918).
  

