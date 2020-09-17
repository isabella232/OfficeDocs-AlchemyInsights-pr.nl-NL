---
title: Regel activiteiten voor Postvak in in auditlogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779046"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="c9568-102">Regel activiteiten voor Postvak in in auditlogboeken</span><span class="sxs-lookup"><span data-stu-id="c9568-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="c9568-103">U kunt zoeken in auditlogboeken gebruiken in de Microsoft 365-beveiligings & nalevings centrum voor het weergeven van regels voor Postvak in-regels (regels voor Postvak in maken, wijzigen en verwijderen).</span><span class="sxs-lookup"><span data-stu-id="c9568-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="c9568-104">Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c9568-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c9568-105">Ga **naar de pagina zoeken in**het  >  **audit logboek** .</span><span class="sxs-lookup"><span data-stu-id="c9568-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c9568-106">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="c9568-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="c9568-107">Controleer onder activiteiten van het **Exchange-postvak**de optie het veld **activiteiten** is ingesteld op **Nieuw-InboxRule de regel voor Postvak in maken/wijzigen/inschakelen/uitschakelen**.</span><span class="sxs-lookup"><span data-stu-id="c9568-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="c9568-108">Klik op **zoeken**.</span><span class="sxs-lookup"><span data-stu-id="c9568-108">Click **Search**.</span></span>

<span data-ttu-id="c9568-109">Selecteer een controlerecord in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="c9568-109">In the results, select an audit record.</span></span> <span data-ttu-id="c9568-110">Klik in het vervolgmenu Details op **meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="c9568-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c9568-111">Informatie over de regelinstellingen voor Postvak in wordt weergegeven in het veld **parameters** .</span><span class="sxs-lookup"><span data-stu-id="c9568-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="c9568-112">Zie [bepalen of een gebruiker een regel voor Postvak in maakt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c9568-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
