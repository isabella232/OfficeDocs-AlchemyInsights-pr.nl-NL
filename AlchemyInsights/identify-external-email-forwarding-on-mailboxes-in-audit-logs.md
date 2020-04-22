---
title: Externe e-maildoorsturen identificeren op postvakken in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716455"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c3348-102">Identificeren wanneer externe e-maildoorsturen is geconfigureerd op postvakken</span><span class="sxs-lookup"><span data-stu-id="c3348-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c3348-103">Wanneer een Microsoft 365-gebruiker externe e-maildoorsturen in een postvak configureert, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="c3348-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c3348-104">U de activiteit bekijken met behulp van zoeken in het controlelogboek in het Beveiligings& Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="c3348-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c3348-105">Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c3348-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c3348-106">Ga naar de**zoekpagina van het zoekcontrolelogboek.** **Search** > </span><span class="sxs-lookup"><span data-stu-id="c3348-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c3348-107">Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.**</span><span class="sxs-lookup"><span data-stu-id="c3348-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c3348-108">U hoeft geen gebruikersnaam op te geven.</span><span class="sxs-lookup"><span data-stu-id="c3348-108">You don't need to specify a username.</span></span> <span data-ttu-id="c3348-109">Controleer of het veld **Activiteiten** is ingesteld op **Resultaten weergeven voor alle activiteiten**.</span><span class="sxs-lookup"><span data-stu-id="c3348-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c3348-110">Klik **op Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="c3348-110">Click **Search**.</span></span>

<span data-ttu-id="c3348-111">Klik in de resultaten op **Resultaten filteren** en typ **Set-Mailbox** in het vak activiteitsfilter.</span><span class="sxs-lookup"><span data-stu-id="c3348-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c3348-112">Selecteer een controlerecord in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="c3348-112">Select an audit record in the results.</span></span> <span data-ttu-id="c3348-113">Klik in de flyout **Details** op **Meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="c3348-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c3348-114">Je moet kijken naar de details van elke audit record om te bepalen of de activiteit is gerelateerd aan e-mail doorsturen.</span><span class="sxs-lookup"><span data-stu-id="c3348-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c3348-115">**ObjectId:** de aliaswaarde van het postvak dat is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c3348-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c3348-116">**Parameters**: _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.</span><span class="sxs-lookup"><span data-stu-id="c3348-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c3348-117">**UserId:** de gebruiker die e-mail doorsturen heeft geconfigureerd in het postvak in het **veld ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="c3348-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c3348-118">Zie [Bepalen wie e-mail doorsturen voor een postvak heeft ingesteld voor](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c3348-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
