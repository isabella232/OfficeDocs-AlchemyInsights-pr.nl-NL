---
title: Regelactiviteit in postvak IN identificeren in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716419"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="f3ef1-102">Regelactiviteit in postvak IN identificeren in controlelogboeken</span><span class="sxs-lookup"><span data-stu-id="f3ef1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="f3ef1-103">U zoeken naar controlelogboeken gebruiken in het Microsoft 365 Security & Compliance Center om regelgebeurtenissen in postvak IN weer te geven (regels voor postvak IN maken, wijzigen en verwijderen).</span><span class="sxs-lookup"><span data-stu-id="f3ef1-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="f3ef1-104">Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f3ef1-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f3ef1-105">Ga naar de**zoekpagina van het zoekcontrolelogboek.** **Search** > </span><span class="sxs-lookup"><span data-stu-id="f3ef1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f3ef1-106">Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.**</span><span class="sxs-lookup"><span data-stu-id="f3ef1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="f3ef1-107">Controleer onder **Exchange-postvakactiviteiten**of het veld **Activiteiten** is ingesteld op **regel Nieuw-InboxRegel maken/wijzigen/inschakelen/uitschakelen**.</span><span class="sxs-lookup"><span data-stu-id="f3ef1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="f3ef1-108">Klik **op Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="f3ef1-108">Click **Search**.</span></span>

<span data-ttu-id="f3ef1-109">Selecteer in de resultaten een controlerecord.</span><span class="sxs-lookup"><span data-stu-id="f3ef1-109">In the results, select an audit record.</span></span> <span data-ttu-id="f3ef1-110">Klik in de flyout met details op **Meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="f3ef1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f3ef1-111">Informatie over de regelinstellingen van het postvak IN wordt weergegeven in het veld **Parameters.**</span><span class="sxs-lookup"><span data-stu-id="f3ef1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="f3ef1-112">Zie [Bepalen of een gebruiker een inboxregel heeft gemaakt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) voor meer informatie</span><span class="sxs-lookup"><span data-stu-id="f3ef1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
