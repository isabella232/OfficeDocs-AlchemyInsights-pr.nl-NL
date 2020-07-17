---
title: PowerShell gebruiken voor het delen van beleidsregels en organisatierelaties
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862055"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="08b2b-102">PowerShell gebruiken voor het delen van beleidsregels en organisatierelaties</span><span class="sxs-lookup"><span data-stu-id="08b2b-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="08b2b-103">Voor organisatierelaties u de gedetailleerde syntaxis- en parameterinformatie controleren voor : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="08b2b-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="08b2b-104">Als u beleid voor delen wilt maken, gebruikt u [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="08b2b-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="08b2b-105">Als [u een beleid voor delen wilt toepassen op een postvak of gebruiker,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) moet u een combinatie van [Set-Postvak](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) en [Postvak maken](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) gebruiken met het nieuw gemaakte beleid.</span><span class="sxs-lookup"><span data-stu-id="08b2b-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="08b2b-106">Als u een deelbeleid wilt [wijzigen, uitschakelen of verwijderen,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) moet u [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) en [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)gebruiken.</span><span class="sxs-lookup"><span data-stu-id="08b2b-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="08b2b-107">**Voor volledig begrip van dit onderwerp u lezen:**</span><span class="sxs-lookup"><span data-stu-id="08b2b-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="08b2b-108">Delen in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="08b2b-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)