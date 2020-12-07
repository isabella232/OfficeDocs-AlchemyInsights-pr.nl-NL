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
# <a name="rbac-rules"></a>RBAC-regels

Als u de machtigingsfout krijgt: 

- **De client met object-id heeft geen autorisatie om actie uit te voeren over het bereik (code: AuthorizationFailed)**: wanneer u een resource probeert te maken, controleert u of u momenteel bent aangemeld met een gebruiker aan wie de rol voor schrijven voor de resource is toegewezen. Als u bijvoorbeeld virtuele machines wilt beheren in een resourcegroep, moet u beschikken over de rol van beheerder van [virtuele machine](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) voor de bronnengroep (of bovenliggend bereik). Zie [ingebouwde rollen voor Azure-bronnen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)voor een lijst met machtigingen voor elke ingebouwde rol.
- **U bent niet gemachtigd om een ondersteuningsaanvraag te maken**: wanneer u probeert een ondersteuningsticket te maken of bij te werken, controleert u of u momenteel bent aangemeld met een gebruiker aan wie de rol Microsoft. support/supportTickets/schrijfbevoegdheid is [toegewezen.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- **Er kunnen geen rollen worden gemaakt (code: RoleAssignmentLimitExceeded)**: wanneer u probeert een rol toe te wijzen, kunt u het aantal roltoewijzingen verlagen door rollen toe te wijzen aan groepen. Azure biedt ondersteuning voor **2000** -roltoewijzingen per abonnement.

Zie voor meer informatie [over Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)-rollen.
