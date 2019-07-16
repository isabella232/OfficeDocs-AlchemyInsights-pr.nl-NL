---
title: Wijziging wachtwoord vereist
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701579"
---
# <a name="change-strong-password-requirement"></a>Wijziging wachtwoord vereist

Sterke wachtwoorden zijn vereist voor standaard. 

Met PowerShell kunt u sterke wachtwoorden gebruikt voor bepaalde gebruikers met deze opdracht uitschakelen:<br>
*Set MsolUser UserPrincipalName – <UserPrincipalName> – StrongPasswordRequired $false*

- [Meer informatie over wachtwoordbeleid](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Verbinding maken met O365 met PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Meer informatie over PowerShell MsolUser-opdrachten](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)