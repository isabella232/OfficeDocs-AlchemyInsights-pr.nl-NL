---
title: Sterke wachtwoordvereisten wijzigen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804418"
---
# <a name="change-strong-password-requirement"></a>Sterke wachtwoordvereisten wijzigen

Voor Microsoft is standaard sterke wachtwoorden vereist.

Met behulp van PowerShell kunt u sterke wachtwoorden voor specifieke gebruikers uitschakelen met de volgende opdrachten:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Gebruik de volgende stappen om sterke wachtwoorden voor alle gebruikers uit te schakelen:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Meer informatie over wachtwoordbeleid](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Verbinding maken met Microsoft 365 met PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Meer informatie over PowerShell MsolUser-opdrachten](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
