---
title: Het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756552"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen

U kunt het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen via het [Microsoft 365-beheercentrum](https://admin.microsoft.com/). Selecteer de groep en kies @bewerken e-mailadres.

U kunt ook de volgende EXO PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep/Teams te wijzigen:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Voorbeeld:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
