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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283613"
---
# <a name="enable-mailbox-auditing"></a>Postvak-controle inschakelen

Om een postbus controle inschakelen voor één gebruiker of een gehele organisatie moet de volgende cmdlets worden uitgevoerd vanuit externe Power Shell:
  
 **Eén gebruiker**
  
Set-Mailbox - identiteit "Jane Dow" - AuditEnabled $true
  
 **Organisatie**
  
Get-Mailbox - ResultSize onbeperkt - Filter {RecipientTypeDetails - eq "UserMailbox"} | $True set-Mailbox - AuditEnabled
  
[Meer informatie](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

