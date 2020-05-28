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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="97b18-102">E-mailadres van een Microsoft 365-groep wijzigen</span><span class="sxs-lookup"><span data-stu-id="97b18-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="97b18-103">U het e-mailadres van een Microsoft 365-groep wijzigen met behulp van het beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="97b18-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="97b18-104">Selecteer de groep en selecteer @edit e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="97b18-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="97b18-105">U ook de opdracht EXO PowerShell gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:</span><span class="sxs-lookup"><span data-stu-id="97b18-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="97b18-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAdres<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="97b18-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="97b18-107">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="97b18-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
