---
title: PowerShell gebruiken voor deelbeleid en organisatierelaties
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
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998461"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShell gebruiken voor deelbeleid en organisatierelaties


Controleer de gedetailleerde syntaxis en parameterinformatie van organisatierelaties voor: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) en [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Gebruik [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) om een nieuw deelbeleid te maken. Je hebt een combinatie van [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) en [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) nodig bij het nieuw aangemaakte beleid om [een deelbeleid op een postvak of gebruiker toe te passen](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes). Gebruik [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) en [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) om [een deelbeleid aan te passen, uit te schakelen of te verwijderen](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy).

**Voor een volledig begrip van dit onderwerp, lees:**

[Delen in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)