---
title: Logboeken beheren
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744379"
---
# <a name="manage-journaling"></a><span data-ttu-id="34509-102">Logboeken beheren</span><span class="sxs-lookup"><span data-stu-id="34509-102">Manage journaling</span></span>

<span data-ttu-id="34509-103">Logboekregistratie kan uw organisatie helpen om te reageren op wettelijke, wettelijke en organisatorische nalevingsvereisten door inkomende en uitgaande e-mailcommunicatie op te nemen.</span><span class="sxs-lookup"><span data-stu-id="34509-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="34509-104">Houd er rekening mee:</span><span class="sxs-lookup"><span data-stu-id="34509-104">Keep in mind:</span></span>

* <span data-ttu-id="34509-105">U moet de machtiging [Organisatiebeheer](https://go.microsoft.com/fwlink/?linkid=2115259) en [Recordsbeheer](https://go.microsoft.com/fwlink/?linkid=2115469) hebben voordat u logboekbeheer kunt beheren.</span><span class="sxs-lookup"><span data-stu-id="34509-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="34509-106">U moet een logboekpostvak en (eventueel) een alternatief postvak voor logboekregistratie hebben geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="34509-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="34509-107">Zie Logboekregistratie configureren in Exchange Online voor [meer informatie.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="34509-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="34509-108">In Exchange Online geldt een limiet voor het aantal logboekregels dat u kunt maken.</span><span class="sxs-lookup"><span data-stu-id="34509-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="34509-109">Zie Regellimieten [voor logboeken, transport en Postvak IN](https://go.microsoft.com/fwlink/?linkid=2115261)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="34509-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="34509-110">Exchange Online biedt geen ondersteuning voor het leveren van logboekrapporten aan een Exchange Online-postvak.</span><span class="sxs-lookup"><span data-stu-id="34509-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="34509-111">U moet het e-mailadres van een on-premises archiveringssysteem of een archiveringsservice van derden opgeven als het postvak voor logboeken.</span><span class="sxs-lookup"><span data-stu-id="34509-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
