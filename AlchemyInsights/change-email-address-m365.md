---
title: E-mailadres van Microsoft 365-groep wijzigen
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461829"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Het e-mailadres van een Microsoft 365-groep wijzigen

Met het Beheercentrum kunt u het e-mailadres van een Microsoft 365-groep wijzigen. Selecteer alleen de groep en selecteer @edit e-mailadres.

U kunt ook de volgen van de EXO PowerShell-opdracht gebruiken voor het wijzigen van het primaire SMTP-adres van een Microsoft 365-groep:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Voorbeeld:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
