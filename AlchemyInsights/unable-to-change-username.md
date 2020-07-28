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
# <a name="unable-to-change-username"></a>Kan gebruikersnaam niet wijzigen

In sommige gevallen worden UPN-wijzigingen (UserPrincipalName) niet doorgegeven aan de cloud. Mogelijk ontvangt u validatiefouten in de Office 365-portal of u de gebruikersnaam of het e-mailadres niet wijzigen. Als u dit probleem wilt oplossen, stelt u UserPrincipalName handmatig in met deze PowerShell-opdracht.

**Voorbeeld: een gebruiker de naam wijzigen**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Met deze opdracht wordt de naam van davidc@contoso.com davidchew@contoso.com.

Zie [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)voor meer informatie.