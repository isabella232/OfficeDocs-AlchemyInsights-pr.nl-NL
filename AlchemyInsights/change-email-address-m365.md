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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="6e627-102">Het e-mailadres van een Microsoft 365-groep wijzigen</span><span class="sxs-lookup"><span data-stu-id="6e627-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="6e627-103">Met het Beheercentrum kunt u het e-mailadres van een Microsoft 365-groep wijzigen.</span><span class="sxs-lookup"><span data-stu-id="6e627-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="6e627-104">Selecteer alleen de groep en selecteer @edit e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="6e627-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="6e627-105">U kunt ook de volgen van de EXO PowerShell-opdracht gebruiken voor het wijzigen van het primaire SMTP-adres van een Microsoft 365-groep:</span><span class="sxs-lookup"><span data-stu-id="6e627-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="6e627-106">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="6e627-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
