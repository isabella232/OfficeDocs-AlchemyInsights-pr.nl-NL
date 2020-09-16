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
# <a name="enable-mailbox-auditing"></a>Controle van Postvak inschakelen

Als u controle van postvak wilt inschakelen voor één gebruiker of voor de hele organisatie, moeten de volgende cmdlets worden uitgevoerd vanaf een externe Power shell:
  
 **Eén gebruiker**
  
Set-mailbox-Identity "Jane Dow"-AuditEnabled $true
  
 **Organisatie**
  
Get-Mailbox-ResultSize Limited-filter {RecipientTypeDetails-EQ "User Mailbox"} | Set-mailbox-AuditEnabled $true
  
[Meer informatie](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

