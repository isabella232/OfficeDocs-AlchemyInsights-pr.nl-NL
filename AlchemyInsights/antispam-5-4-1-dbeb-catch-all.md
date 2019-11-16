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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672428"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="285bc-102">Leveringsproblemen oplossen voor foutcode 550 5.4.1 relaytoegang geweigerd</span><span class="sxs-lookup"><span data-stu-id="285bc-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="285bc-103">Dit probleem treedt op bij het [controleren om te zien of een e-mailadres geldig is om te voorkomen dat bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) bij het invoeren van het netwerk van Office 365.</span><span class="sxs-lookup"><span data-stu-id="285bc-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="285bc-104">Probeer het volgende:</span><span class="sxs-lookup"><span data-stu-id="285bc-104">Try the following:</span></span>

1. <span data-ttu-id="285bc-105">Bepaal of het probleem specifiek is voor een volledig domein of voor één e-mailadres:</span><span class="sxs-lookup"><span data-stu-id="285bc-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="285bc-106">Hele domein: soms moet het domein worden gesynchroniseerd; Probeer [het domein in te stellen op intern en vervolgens terug naar gezaghebbend](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="285bc-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="285bc-107">Eén e-mailadres: soms moet het adres worden gesynchroniseerd; Als u het SMTP-proxyadres wijzigt en vervolgens weer wijzigt, kan dit helpen.</span><span class="sxs-lookup"><span data-stu-id="285bc-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="285bc-108">Bepaal of het probleem specifiek is voor een groep of openbare map.</span><span class="sxs-lookup"><span data-stu-id="285bc-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="285bc-109">Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="285bc-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="285bc-110">Als u extra hulp nodig hebt, opent u een ondersteuningsticket en geeft u het bereik van het probleem op (includidng het type object waarnaar u verzendt), zodat we u beter kunnen helpen.</span><span class="sxs-lookup"><span data-stu-id="285bc-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>