---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821442"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="64591-102">Bezorgingsproblemen oplossen voor foutcode 550 5.4.1 Doorlevertoegang geweigerd</span><span class="sxs-lookup"><span data-stu-id="64591-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="64591-103">Dit probleem treedt op bij het controleren of een e-mailadres geldig is om [stuiterbacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) te voorkomen bij het invoeren van het Microsoft-netwerk.</span><span class="sxs-lookup"><span data-stu-id="64591-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="64591-104">Probeer het volgende:</span><span class="sxs-lookup"><span data-stu-id="64591-104">Try the following:</span></span>

1. <span data-ttu-id="64591-105">Bepaal of het probleem specifiek is voor een heel domein of één e-mailadres:</span><span class="sxs-lookup"><span data-stu-id="64591-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="64591-106">Hele domein: Soms moet het domein worden gesynchroniseerd. probeer [het domein in te stellen op Intern en vervolgens terug te gaan naar Gezaghebbend.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="64591-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="64591-107">Eén e-mailadres: Soms moet het adres worden gesynchroniseerd; het wijzigen van het smtp-proxyadres en het vervolgens wijzigen van het adres kan helpen.</span><span class="sxs-lookup"><span data-stu-id="64591-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="64591-108">Bepaal of het probleem specifiek is voor een groep of openbare map.</span><span class="sxs-lookup"><span data-stu-id="64591-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="64591-109">Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="64591-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="64591-110">Als u extra hulp nodig hebt, opent u een ondersteuningsticket en geeft u het bereik van het probleem op (inclusief het type object dat u wilt verzenden) zodat we u beter kunnen helpen.</span><span class="sxs-lookup"><span data-stu-id="64591-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>