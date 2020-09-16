---
title: Dagelijkse e-mail limiet is overschreden. Werkstroom is opgeschort.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731558"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="43c36-103">Dagelijkse e-mail limiet is overschreden.</span><span class="sxs-lookup"><span data-stu-id="43c36-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="43c36-104">Werkstroom is opgeschort.</span><span class="sxs-lookup"><span data-stu-id="43c36-104">Workflow is suspended.</span></span>

<span data-ttu-id="43c36-105">Deze fout kan worden weergegeven in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="43c36-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="43c36-106">U hebt een werkstroom in SharePoint Online die het type SharePoint 2010 of SharePoint 2013-werkstroom platform gebruikt.</span><span class="sxs-lookup"><span data-stu-id="43c36-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="43c36-107">De werkstroom is geconfigureerd voor het verzenden van een aangepast e-mailbericht naar meer dan 200 gebruikers tegelijk, meer dan 10.000 geadresseerden per dag, of meer dan 30 berichten per minuut.</span><span class="sxs-lookup"><span data-stu-id="43c36-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="43c36-108">Wanneer u de werkstroom uitvoert, wordt het e-mailbericht niet verzonden en ziet u het volgende gedrag:</span><span class="sxs-lookup"><span data-stu-id="43c36-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="43c36-109">Voor een werkstroom met het platformtype SharePoint 2013, bladert u naar de pagina **werkstroom status** .</span><span class="sxs-lookup"><span data-stu-id="43c36-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="43c36-110">Op de pagina werkstroom status wordt de **interne status** ingesteld op **gestart**en wordt de informatie ballon **niet naar een geadresseerde verzonden**.</span><span class="sxs-lookup"><span data-stu-id="43c36-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="43c36-111">Om dit probleem tijdelijk op te lossen, configureert u uw werkstroom voor het verzenden van e-mailberichten zonder dat de [afzenders van Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)worden overschreden</span><span class="sxs-lookup"><span data-stu-id="43c36-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="43c36-112">Met een onderbreking in de werkstroom kunt u bijvoorbeeld de e-mail verzenden naar een Microsoft 365-groep, een distributiegroep of een beveiligingsgroep met e-mail, of het bericht verzenden naar minder dan 200 geadresseerden tegelijk.</span><span class="sxs-lookup"><span data-stu-id="43c36-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="43c36-113">Zie het volgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="43c36-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="43c36-114">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="43c36-114">Related topics</span></span>
- [<span data-ttu-id="43c36-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="43c36-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="43c36-116">SharePoint en flow</span><span class="sxs-lookup"><span data-stu-id="43c36-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 