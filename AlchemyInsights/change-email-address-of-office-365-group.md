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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580652"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>E-mailadres van een Microsoft 365-groep wijzigen

U het e-mailadres van een Microsoft 365-groep wijzigen met behulp van het beheercentrum. Selecteer de groep en selecteer @edit e-mailadres.

U de opdracht EXO PowerShell ook gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Voorbeeld:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
