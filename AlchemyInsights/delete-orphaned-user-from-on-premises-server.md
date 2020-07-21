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
# <a name="delete-orphaned-user-from-on-premises-server"></a>Verweesde gebruiker verwijderen van on-premises server

Voer de volgende stappen uit om een verweesde gebruiker te verwijderen:

1. Directorysynchronisatie forceren door de instructies op te volgen in [Wat is hybride identiteit met Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. Zie [Wat is hybride identiteit met Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx)

3. Als synchronisatie correct werkt, maar de verwijdering van Active Directory-objecten niet wordt doorgegeven aan Azure AD, verwijdert u het verweesde object handmatig met behulp van een van de volgende Azure Active Directory Module voor Windows PowerShell-cmdlets:

    Contact verwijderen-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Als u bijvoorbeeld de status van verlaten gebruikers-id john.smith@contoso.com wilt verwijderen, oorspronkelijk gemaakt met behulp van adreslijstsynchronisatie, voert u de cmdlet uit:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com