---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707906"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="6967f-102">Leveringsproblemen oplossen voor foutcode 550 5.4.1 Relay-toegang geweigerd</span><span class="sxs-lookup"><span data-stu-id="6967f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="6967f-103">Dit probleem treedt op bij [het controleren of een e-mailadres geldig is om bouncebacks te voorkomen](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) bij het invoeren van het Microsoft-netwerk.</span><span class="sxs-lookup"><span data-stu-id="6967f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="6967f-104">Probeer het volgende:</span><span class="sxs-lookup"><span data-stu-id="6967f-104">Try the following:</span></span>

1. <span data-ttu-id="6967f-105">Bepaal of het probleem specifiek is voor een heel domein of één e-mailadres:</span><span class="sxs-lookup"><span data-stu-id="6967f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="6967f-106">Hele domein: Soms moet het domein worden gesynchroniseerd; probeer [het domein in te stellen op Intern en vervolgens terug naar Gezaghebbend](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="6967f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="6967f-107">Eén e-mailadres: Soms moet het adres worden gesynchroniseerd; het wijzigen van de smtp proxy-adres en vervolgens het veranderen van het terug kan helpen.</span><span class="sxs-lookup"><span data-stu-id="6967f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="6967f-108">Bepaal of het probleem specifiek is voor een groep of openbare map.</span><span class="sxs-lookup"><span data-stu-id="6967f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="6967f-109">Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6967f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="6967f-110">Als je extra hulp nodig hebt, open dan een ondersteuningsticket en geef de omvang van het probleem op (inclusief het type object waarnaar je stuurt) zodat we je beter kunnen helpen.</span><span class="sxs-lookup"><span data-stu-id="6967f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>