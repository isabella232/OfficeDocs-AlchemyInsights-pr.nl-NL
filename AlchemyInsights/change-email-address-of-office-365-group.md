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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="e3767-102">Het e-mailadres van een Microsoft 365-groep wijzigen</span><span class="sxs-lookup"><span data-stu-id="e3767-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="e3767-103">U kunt het e-mailadres van een Microsoft 365-groep wijzigen via het beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="e3767-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="e3767-104">Selecteer de groep en kies @bewerken e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="e3767-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="e3767-105">U kunt ook de EXO Windows PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:</span><span class="sxs-lookup"><span data-stu-id="e3767-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="e3767-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="e3767-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="e3767-107">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="e3767-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
