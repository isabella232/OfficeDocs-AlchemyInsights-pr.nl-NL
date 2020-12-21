---
title: AggregateGroupMailbox volledige NDR ontvangen voor e-mail verzonden naar Microsoft 365-groep
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721822"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox volledige NDR ontvangen voor e-mail verzonden naar Microsoft 365-groep

Gebruik de volgende shell-opdracht van EXO om een Exchange-transportregel te maken voor het doorsturen van e-mailberichten die zijn verzonden naar het groeps Postvak

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Vervang het SMTP-adres in **-SentTo** met SMTP-adres van het groeps postvak van de samenvoeging in uw Tenant. U kunt het SMTP-adres van het groeps postvak voor de samenvoeging openen via de NDR ontvangen.



