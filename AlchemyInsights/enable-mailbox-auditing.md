---
title: Controle van postvakken inschakelen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506949"
---
# <a name="enable-mailbox-auditing"></a>Controle van postvakken inschakelen

Als u Postvakcontrole voor één gebruiker of een hele organisatie wilt inschakelen, moeten de volgende cmdlets worden uitgevoerd vanuit Remote Power Shell:
  
 **Eén gebruiker**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Organisatie**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-mailbox -AuditEnabled $true
  
[Meer informatie](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

