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
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826050"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="9ee0f-102">PowerShell gebruiken voor deelbeleid en organisatierelaties</span><span class="sxs-lookup"><span data-stu-id="9ee0f-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="9ee0f-103">Controleer de gedetailleerde syntaxis en parameterinformatie van organisatierelaties voor: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) en [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="9ee0f-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="9ee0f-104">Gebruik [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) om een nieuw deelbeleid te maken.</span><span class="sxs-lookup"><span data-stu-id="9ee0f-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="9ee0f-105">Je hebt een combinatie van [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) en [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) nodig bij het nieuw aangemaakte beleid om [een deelbeleid op een postvak of gebruiker toe te passen](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="9ee0f-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="9ee0f-106">Gebruik [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) en [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) om [een deelbeleid aan te passen, uit te schakelen of te verwijderen](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy).</span><span class="sxs-lookup"><span data-stu-id="9ee0f-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="9ee0f-107">**Voor een volledig begrip van dit onderwerp, lees:**</span><span class="sxs-lookup"><span data-stu-id="9ee0f-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="9ee0f-108">Delen in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="9ee0f-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)