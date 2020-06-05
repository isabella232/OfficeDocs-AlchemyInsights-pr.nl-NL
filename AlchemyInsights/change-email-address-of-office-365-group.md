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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b4a55-102">E-mailadres van een Microsoft 365-groep wijzigen</span><span class="sxs-lookup"><span data-stu-id="b4a55-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b4a55-103">U het e-mailadres van een Microsoft 365-groep wijzigen met behulp van het beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="b4a55-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b4a55-104">Selecteer de groep en selecteer @edit e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="b4a55-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b4a55-105">U de opdracht EXO PowerShell ook gebruiken om het primaire SMTP-adres van een Microsoft 365-groep te wijzigen:</span><span class="sxs-lookup"><span data-stu-id="b4a55-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="b4a55-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b4a55-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b4a55-107">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="b4a55-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
