---
title: Beleid voor het delen van agenda's
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372994"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="ac220-102">Beleidsfout bij het delen van een agenda</span><span class="sxs-lookup"><span data-stu-id="ac220-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="ac220-103">Doe een van de volgende handelingen, naar gelang van het geval voor uw situatie:</span><span class="sxs-lookup"><span data-stu-id="ac220-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="ac220-104">Maak verbinding met Exchange Online met Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ac220-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="ac220-105">Zie [Verbinding maken met Exchange Online met Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ac220-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="ac220-106">Open de Exchange Management Shell op de on-premises server.</span><span class="sxs-lookup"><span data-stu-id="ac220-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="ac220-107">Bepaal het beleid voor delen dat aan de gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="ac220-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="ac220-108">Voer hiervoor de volgende opdracht uit en noteer het geretourneerde beleid:</span><span class="sxs-lookup"><span data-stu-id="ac220-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="ac220-109">Werk het beleid voor delen voor de gebruiker bij.</span><span class="sxs-lookup"><span data-stu-id="ac220-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="ac220-110">Volg deze stappen om dit te doen:</span><span class="sxs-lookup"><span data-stu-id="ac220-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="ac220-111">Open het Exchange-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ac220-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="ac220-112">Klik **op Organisatie**en dubbelklik op het beleid dat aan de gebruiker is toegewezen onder Individueel **delen**.</span><span class="sxs-lookup"><span data-stu-id="ac220-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="ac220-113">Dit is het beleid dat is geretourneerd in stap 2.</span><span class="sxs-lookup"><span data-stu-id="ac220-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="ac220-114">Selecteer op de pagina Regel delen het niveau voor het delen van agenda's dat u wilt toestaan onder **Opgeven welke informatie u wilt delen**; klik **op Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="ac220-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="ac220-115">Voor meer informatie zie: ["Beleid staat niet toe dat machtigingen op dit niveau worden verleend aan een of meer van de ontvanger(s)" fout wanneer de gebruiker probeert om agenda te delen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="ac220-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
