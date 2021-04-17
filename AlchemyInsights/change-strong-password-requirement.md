---
title: Sterke wachtwoordvereiste wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818463"
---
# <a name="change-strong-password-requirement"></a>Sterke wachtwoordvereiste wijzigen

Microsoft vereist standaard sterke wachtwoorden.

Met PowerShell kunt u sterke wachtwoorden voor specifieke gebruikers uitschakelen met deze opdrachten:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Gebruik de volgende functies om sterke wachtwoorden voor alle gebruikers uit te schakelen:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Meer informatie over wachtwoordbeleid](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Verbinding maken met Microsoft 365 met PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Meer informatie over PowerShell MsolUser-opdrachten](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
