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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930724"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Het e-mailadres van een Microsoft 365-groep wijzigen

U kunt het e-mailadres van een Microsoft 365-groep wijzigen via het beheercentrum. Selecteer de groep en kies @bewerken e-mailadres.

U kunt ook de EXO Windows PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Voorbeeld:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
