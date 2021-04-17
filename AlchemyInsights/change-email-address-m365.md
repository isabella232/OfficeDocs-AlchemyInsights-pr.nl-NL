---
title: Het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819075"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="a249c-102">Het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen</span><span class="sxs-lookup"><span data-stu-id="a249c-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="a249c-103">U kunt het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen via het [Microsoft 365-beheercentrum](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a249c-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="a249c-104">Selecteer de groep en kies @bewerken e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="a249c-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a249c-105">U kunt ook de volgende EXO PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep/Teams te wijzigen:</span><span class="sxs-lookup"><span data-stu-id="a249c-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="a249c-106">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="a249c-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
