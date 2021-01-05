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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="ab62f-102">Het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen</span><span class="sxs-lookup"><span data-stu-id="ab62f-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="ab62f-103">U kunt het e-mailadres van een Microsoft 365-groep of Microsoft Teams wijzigen via het [Microsoft 365-beheercentrum](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ab62f-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="ab62f-104">Selecteer de groep en kies @bewerken e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="ab62f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="ab62f-105">U kunt ook de volgende EXO PowerShell-opdracht gebruiken om het primaire SMTP-adres van een Microsoft 365-groep/Teams te wijzigen:</span><span class="sxs-lookup"><span data-stu-id="ab62f-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="ab62f-106">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="ab62f-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
