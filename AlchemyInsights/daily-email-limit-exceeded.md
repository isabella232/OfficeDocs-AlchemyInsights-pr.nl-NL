---
title: Dagelijkse e-mail limiet overschreden. Workflow is geschorst.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514442"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="8dd0c-103">Dagelijkse e-mail limiet overschreden.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="8dd0c-104">Workflow is geschorst.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-104">Workflow is suspended.</span></span>

<span data-ttu-id="8dd0c-105">Deze fout kan worden ontvangen in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="8dd0c-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="8dd0c-106">U hebt een werkstroom in SharePoint Online die de SharePoint 2010 of SharePoint 2013 workflow platform wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="8dd0c-107">De werkstroom is geconfigureerd voor een aangepast e-mailbericht verzenden naar meer dan 200 gebruikers op een moment, meer dan 10.000 geadresseerden per dag of meer dan 30 berichten per minuut.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="8dd0c-108">Tijdens het uitvoeren van de werkstroom het e-mailbericht niet verzonden en u ziet het volgende gedrag:</span><span class="sxs-lookup"><span data-stu-id="8dd0c-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="8dd0c-109">U bladert naar de pagina **Werkstroomstatus** voor een werkstroom met behulp van het type SharePoint 2013-platform.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="8dd0c-110">De **Interne Status** is ingesteld op **gestart**en de ballon van de informatie **kan niet worden verzonden naar een geadresseerde**wordt weergegeven op de pagina Werkstroomstatus.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="8dd0c-111">U kunt dit probleem omzeilen, kunt u uw workflow voor het verzenden van e-mailberichten zonder overschrijding van de [grenzen van Exchange Online afzender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)configureren.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="8dd0c-112">Bijvoorbeeld een pauze in de workflow gebruikt het e-mailbericht verzenden naar een Office 365-groep, een distributiegroep of beveiligingsgroep e-mail is ingeschakeld of het bericht naar minder dan 200 geadresseerden per keer verzenden.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="8dd0c-113">Raadpleeg het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8dd0c-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="8dd0c-114">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="8dd0c-114">Related topics</span></span>
- [<span data-ttu-id="8dd0c-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="8dd0c-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8dd0c-116">SharePoint en stroom</span><span class="sxs-lookup"><span data-stu-id="8dd0c-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 