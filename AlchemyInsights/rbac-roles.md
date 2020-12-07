---
title: 'RBAC-rollen '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583352"
---
# <a name="rbac-rules"></a><span data-ttu-id="eaf22-102">RBAC-regels</span><span class="sxs-lookup"><span data-stu-id="eaf22-102">RBAC rules</span></span>

<span data-ttu-id="eaf22-103">Als u de machtigingsfout krijgt:</span><span class="sxs-lookup"><span data-stu-id="eaf22-103">If you get the permission error:</span></span> 

- <span data-ttu-id="eaf22-104">**De client met object-id heeft geen autorisatie om actie uit te voeren over het bereik (code: AuthorizationFailed)**: wanneer u een resource probeert te maken, controleert u of u momenteel bent aangemeld met een gebruiker aan wie de rol voor schrijven voor de resource is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="eaf22-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="eaf22-105">Als u bijvoorbeeld virtuele machines wilt beheren in een resourcegroep, moet u beschikken over de rol van beheerder van [virtuele machine](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) voor de bronnengroep (of bovenliggend bereik).</span><span class="sxs-lookup"><span data-stu-id="eaf22-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="eaf22-106">Zie [ingebouwde rollen voor Azure-bronnen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)voor een lijst met machtigingen voor elke ingebouwde rol.</span><span class="sxs-lookup"><span data-stu-id="eaf22-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="eaf22-107">**U bent niet gemachtigd om een ondersteuningsaanvraag te maken**: wanneer u probeert een ondersteuningsticket te maken of bij te werken, controleert u of u momenteel bent aangemeld met een gebruiker aan wie de rol Microsoft. support/supportTickets/schrijfbevoegdheid is [toegewezen.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)</span><span class="sxs-lookup"><span data-stu-id="eaf22-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="eaf22-108">**Er kunnen geen rollen worden gemaakt (code: RoleAssignmentLimitExceeded)**: wanneer u probeert een rol toe te wijzen, kunt u het aantal roltoewijzingen verlagen door rollen toe te wijzen aan groepen.</span><span class="sxs-lookup"><span data-stu-id="eaf22-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="eaf22-109">Azure biedt ondersteuning voor **2000** -roltoewijzingen per abonnement.</span><span class="sxs-lookup"><span data-stu-id="eaf22-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="eaf22-110">Zie voor meer informatie [over Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)-rollen.</span><span class="sxs-lookup"><span data-stu-id="eaf22-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
