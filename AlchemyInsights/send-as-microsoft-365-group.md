---
title: Verzenden als Microsoft 365-groep
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871730"
---
# <a name="send-as-microsoft-365-group"></a>Verzenden als Microsoft 365-groep

U kunt de machtiging Verzenden als toewijzen, zodat bepaalde gebruikers berichten kunnen verzenden als een Microsoft 365-groep:  

1. Verbinding maken met Exchange Online PowerShell.  

2. Voer de volgende opdracht uit:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights Sendas

Zie [toestaan dat leden e-mail verzenden als of verzenden namens een groep](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)voor meer informatie.