---
title: Beleid voor het delen van een 618-agenda
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684225"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="2fbe7-102">Beleidsfout bij het delen van een agenda</span><span class="sxs-lookup"><span data-stu-id="2fbe7-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="2fbe7-103">Voer een van de volgende handelingen uit, afhankelijk van uw situatie:</span><span class="sxs-lookup"><span data-stu-id="2fbe7-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="2fbe7-104">Maak verbinding met Exchange Online via externe PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="2fbe7-105">Zie [verbinding maken met Exchange Online via externe PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="2fbe7-106">Open de Exchange-beheer shell op de lokale server.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="2fbe7-107">Bepaal het beleid voordelen dat is toegewezen aan de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="2fbe7-108">Als u dit wilt doen, voert u de volgende opdracht uit en noteert u het geretourneerde beleid:</span><span class="sxs-lookup"><span data-stu-id="2fbe7-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="2fbe7-109">Het beleid voor het delen van de gebruiker bijwerken.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="2fbe7-110">Ga hiervoor als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="2fbe7-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="2fbe7-111">Open het Exchange-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="2fbe7-112">Klik op **organisatie**en dubbelklik vervolgens op het beleid dat is toegewezen aan de gebruiker onder **afzonderlijk delen**.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="2fbe7-113">Dit is het beleid dat u in stap 2 hebt geretourneerd.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="2fbe7-114">Selecteer op de pagina regel voordelen het niveau voor het delen van de agenda dat u wilt toestaan onder **opgeven welke gegevens u wilt delen**. Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="2fbe7-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="2fbe7-115">Zie voor meer informatie: [' beleid staat het toekennen van machtigingen op dit niveau toe aan een of meer van de geadresseerde (n) wanneer de gebruiker probeert de agenda te delen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="2fbe7-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
