---
title: Het e-mailadres van een Microsoft 365-groep wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819039"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Het e-mailadres van een Microsoft 365-groep wijzigen

U kunt het e-mailadres van een Microsoft 365-groep wijzigen via het beheercentrum. Selecteer de groep en kies @bewerken e-mailadres.

U kunt ook de EXO Windows PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Voorbeeld:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
