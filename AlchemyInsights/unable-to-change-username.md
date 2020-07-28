---
title: Kan gebruikersnaam niet wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439100"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="186f0-102">Kan gebruikersnaam niet wijzigen</span><span class="sxs-lookup"><span data-stu-id="186f0-102">Unable to change UserName</span></span>

<span data-ttu-id="186f0-103">In sommige gevallen worden UPN-wijzigingen (UserPrincipalName) niet doorgegeven aan de cloud.</span><span class="sxs-lookup"><span data-stu-id="186f0-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="186f0-104">Mogelijk ontvangt u validatiefouten in de Office 365-portal of u de gebruikersnaam of het e-mailadres niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="186f0-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="186f0-105">Als u dit probleem wilt oplossen, stelt u UserPrincipalName handmatig in met deze PowerShell-opdracht.</span><span class="sxs-lookup"><span data-stu-id="186f0-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="186f0-106">**Voorbeeld: een gebruiker de naam wijzigen**</span><span class="sxs-lookup"><span data-stu-id="186f0-106">**Example: Rename a user**</span></span>

<span data-ttu-id="186f0-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="186f0-107">PowerShellCopy</span></span>

<span data-ttu-id="186f0-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="186f0-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="186f0-109">Met deze opdracht wordt de naam van davidc@contoso.com davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="186f0-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="186f0-110">Zie [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="186f0-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>