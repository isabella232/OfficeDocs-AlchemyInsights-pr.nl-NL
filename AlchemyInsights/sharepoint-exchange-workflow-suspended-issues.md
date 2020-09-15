---
title: Aan de slag met SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700702"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="3cfc2-102">Werkstromen in SharePoint</span><span class="sxs-lookup"><span data-stu-id="3cfc2-102">Workflows in SharePoint</span></span>

<span data-ttu-id="3cfc2-103">Als SharePoint-werkstromen geen e-mailberichten verzenden, heeft uw organisatie mogelijk de limieten voor de Exchange Online-afzender vastgesteld.</span><span class="sxs-lookup"><span data-stu-id="3cfc2-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="3cfc2-104">Wanneer u een van de volgende items hebt, wordt het foutbericht ' werkstroom is opgeschort ' weergegeven:</span><span class="sxs-lookup"><span data-stu-id="3cfc2-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="3cfc2-105">U hebt een werkstroom in SharePoint Online die het type SharePoint 2010 of SharePoint 2013-werkstroom platform gebruikt.</span><span class="sxs-lookup"><span data-stu-id="3cfc2-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="3cfc2-106">De werkstroom is geconfigureerd voor het verzenden van een aangepast e-mailbericht naar meer dan 200 gebruikers tegelijk, meer dan 10.000 geadresseerden per dag, of meer dan 30 berichten per minuut.</span><span class="sxs-lookup"><span data-stu-id="3cfc2-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="3cfc2-107">Wanneer u de werkstroom uitvoert, wordt het e-mailbericht niet verzonden en wordt het foutbericht weergegeven en wordt de interne status ingesteld op geschorst of kan de opdracht niet naar een geadresseerde worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="3cfc2-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="3cfc2-108">Raadpleeg het volgende [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="3cfc2-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

