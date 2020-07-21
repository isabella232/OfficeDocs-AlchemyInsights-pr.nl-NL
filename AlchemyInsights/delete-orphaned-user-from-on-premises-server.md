---
title: Verweesde gebruiker verwijderen van on-premises server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197941"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="3e293-102">Verweesde gebruiker verwijderen van on-premises server</span><span class="sxs-lookup"><span data-stu-id="3e293-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="3e293-103">Voer de volgende stappen uit om een verweesde gebruiker te verwijderen:</span><span class="sxs-lookup"><span data-stu-id="3e293-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="3e293-104">Directorysynchronisatie forceren door de instructies op te volgen in [Wat is hybride identiteit met Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)</span><span class="sxs-lookup"><span data-stu-id="3e293-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="3e293-105">Zie [Wat is hybride identiteit met Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="3e293-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="3e293-106">Als synchronisatie correct werkt, maar de verwijdering van Active Directory-objecten niet wordt doorgegeven aan Azure AD, verwijdert u het verweesde object handmatig met behulp van een van de volgende Azure Active Directory Module voor Windows PowerShell-cmdlets:</span><span class="sxs-lookup"><span data-stu-id="3e293-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="3e293-107">Contact verwijderen-MsolContact</span><span class="sxs-lookup"><span data-stu-id="3e293-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="3e293-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="3e293-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="3e293-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="3e293-109">Remove-MsolUser</span></span>

    <span data-ttu-id="3e293-110">Als u bijvoorbeeld de status van verlaten gebruikers-id john.smith@contoso.com wilt verwijderen, oorspronkelijk gemaakt met behulp van adreslijstsynchronisatie, voert u de cmdlet uit:</span><span class="sxs-lookup"><span data-stu-id="3e293-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="3e293-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="3e293-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>