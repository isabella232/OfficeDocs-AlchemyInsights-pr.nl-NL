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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923126"
---
# <a name="rbac-rules"></a>RBAC-regels

Als de machtigingsfout wordt weergegeven: 

- De client met object-id heeft geen machtiging om actie uit te voeren via het bereik **(code: AutorisatieFailed)**: als u een resource probeert te maken, controleert u of u momenteel bent aangemeld bij een gebruiker die een rol heeft toegewezen die schrijfmachtigingen heeft voor de resource in het geselecteerde bereik. Als u bijvoorbeeld virtuele machines in een resourcegroep wilt beheren, moet u de rol Virtual [Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) hebben in de resourcegroep (of bovenliggend bereik). Zie Ingebouwde rollen voor [Azure-resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)voor een lijst met machtigingen voor elke ingebouwde rol.
- U hebt geen machtiging om een ondersteuningsaanvraag te **maken:** wanneer u een ondersteuningsticket probeert te maken of bij te werken, controleert u of u momenteel bent aangemeld bij een gebruiker die een rol heeft toegewezen die de machtiging Microsoft.Support/supportTickets/write heeft, zoals Medewerker ondersteuningsaanvraag. [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Er kunnen geen roltoewijzingen meer worden gemaakt **(code: RoleAssignmentLimitExceeded)**: wanneer u een rol probeert toe te wijzen, probeert u het aantal roltoewijzingen te verminderen door in plaats daarvan rollen toe te wijzen aan groepen. Azure ondersteunt maximaal **2000** roltoewijzingen per abonnement.

Zie Azure RBAC-rollen voor meer informatie over Azure [RBAC-rollen.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
