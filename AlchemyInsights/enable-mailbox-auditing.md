---
title: Postbus controle inschakelen
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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736248"
---
# <a name="enable-mailbox-auditing"></a>Postbus controle inschakelen

Als u wilt inschakelen Postvakcontrole voor een enkele gebruiker of een hele organisatie de volgende cmdlets moeten worden uitgevoerd vanaf een externe Power shell:
  
 **Enkele gebruiker**
  
Set-mailbox-identiteit "Jane Dow"-AuditEnabled $true
  
 **Organisatie**
  
Get-postbus-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-mailbox-AuditEnabled $true
  
[Meer informatie](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

