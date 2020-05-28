---
title: E-mailadres van een Microsoft 365-groep wijzigen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282352"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>E-mailadres van een Microsoft 365-groep wijzigen

U het e-mailadres van een Microsoft 365-groep wijzigen met behulp van het beheercentrum. Selecteer de groep en selecteer @edit e-mailadres.

U ook de opdracht EXO PowerShell gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:

Set-UnifiedGroup <Group Name> -PrimarySmtpAdres<new SMTP Address>

Voorbeeld:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
