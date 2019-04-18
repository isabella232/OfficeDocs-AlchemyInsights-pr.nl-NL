---
title: Externe e-mail doorsturen op postvakken in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909165"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c8840-102">Bepalen wanneer externe e-mail doorsturen is geconfigureerd op de postvakken</span><span class="sxs-lookup"><span data-stu-id="c8840-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c8840-103">Wanneer een gebruiker configureert externe e-mail doorsturen voor een postbus, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="c8840-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c8840-104">Hier ziet u de activiteit met audit-logboek zoeken in de & beveiliging conformiteit.</span><span class="sxs-lookup"><span data-stu-id="c8840-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c8840-105">Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c8840-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c8840-106">Klik op **Zoeken en onderzoek** en **Audit-logboek zoeken**selecteren.</span><span class="sxs-lookup"><span data-stu-id="c8840-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c8840-107">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="c8840-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c8840-108">U hoeft niet een gebruikersnaam opgeven.</span><span class="sxs-lookup"><span data-stu-id="c8840-108">You don't need to specify a username.</span></span> <span data-ttu-id="c8840-109">Controleer of dat de **activiteiten** -veld is ingesteld op het **weergeven van resultaten voor alle activiteiten**.</span><span class="sxs-lookup"><span data-stu-id="c8840-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c8840-110">Klik op **Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="c8840-110">Click **Search**.</span></span>

<span data-ttu-id="c8840-111">In de resultaten, klikt u op **Filterresultaten** en **Set-Postvak** typt in het vak activiteit filter.</span><span class="sxs-lookup"><span data-stu-id="c8840-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c8840-112">Selecteer een audit record in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="c8840-112">Select an audit record in the results.</span></span> <span data-ttu-id="c8840-113">Klik op **meer informatie**in het doel **Details** .</span><span class="sxs-lookup"><span data-stu-id="c8840-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c8840-114">U moet de details van elke record controleren om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.</span><span class="sxs-lookup"><span data-stu-id="c8840-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c8840-115">**Object-id**: de waarde van de alias van het postvak dat is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c8840-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c8840-116">**Parameters**: _ForwardingSmtpAddress_ geeft aan dat het doel-e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="c8840-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c8840-117">**UserId**: de gebruiker die het doorsturen van e-mail in het postvak in in het veld **id** geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="c8840-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c8840-118">Zie [vaststellen die e-mail doorsturen voor een postbus instellen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c8840-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
