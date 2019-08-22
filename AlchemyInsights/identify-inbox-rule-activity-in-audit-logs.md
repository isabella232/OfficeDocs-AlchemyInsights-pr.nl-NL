---
title: Postvak in regel activiteit in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539158"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="f3013-102">Postvak in regel activiteit in de controlelogboeken geïdentificeerd</span><span class="sxs-lookup"><span data-stu-id="f3013-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="f3013-103">Audit-logboek zoeken kunt u in de beveiliging van Office 365 & conformiteit postvak in regel gebeurtenissen (maken, wijzigen en verwijderen van regels voor postvak in) weergeven.</span><span class="sxs-lookup"><span data-stu-id="f3013-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="f3013-104">Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f3013-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f3013-105">Ga naar de **Search** > **Audit log** zoekpagina.</span><span class="sxs-lookup"><span data-stu-id="f3013-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f3013-106">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="f3013-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="f3013-107">Controleer of het veld **activiteiten** is ingesteld onder **Exchange Mailbox activiteiten** **Nieuw InboxRule maken/wijzigen/inschakelen/uitschakelen van de regel voor postvak in**.</span><span class="sxs-lookup"><span data-stu-id="f3013-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="f3013-108">Klik op **Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="f3013-108">Click **Search**.</span></span>

<span data-ttu-id="f3013-109">Selecteer een audit record in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="f3013-109">In the results, select an audit record.</span></span> <span data-ttu-id="f3013-110">Klik op **Meer informatie**in het doel details.</span><span class="sxs-lookup"><span data-stu-id="f3013-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f3013-111">Informatie over de instellingen van het postvak in wordt weergegeven in het veld **Parameters** .</span><span class="sxs-lookup"><span data-stu-id="f3013-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="f3013-112">Zie [vaststellen als een gebruiker die een postvak in-regel gemaakt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f3013-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
