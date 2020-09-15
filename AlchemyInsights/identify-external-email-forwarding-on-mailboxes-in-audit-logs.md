---
title: Externe e-mailberichten doorsturen naar postvakken in controlelogboeken
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696292"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="39e13-102">Identificeren wanneer externe e-mail forwarding is geconfigureerd voor postvakken</span><span class="sxs-lookup"><span data-stu-id="39e13-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="39e13-103">Wanneer een Microsoft 365-gebruiker externe e-mail forwarding configureert voor een postvak, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **set-mailbox** .</span><span class="sxs-lookup"><span data-stu-id="39e13-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="39e13-104">U kunt de activiteit zien met de zoekfunctie voor auditlogboeken in de beveiligings & compliance Center.</span><span class="sxs-lookup"><span data-stu-id="39e13-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="39e13-105">Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="39e13-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="39e13-106">Ga **naar de pagina zoeken in**het  >  **audit logboek** .</span><span class="sxs-lookup"><span data-stu-id="39e13-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="39e13-107">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="39e13-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="39e13-108">U hoeft geen gebruikersnaam op te geven.</span><span class="sxs-lookup"><span data-stu-id="39e13-108">You don't need to specify a username.</span></span> <span data-ttu-id="39e13-109">Controleer of het veld **activiteiten** is ingesteld op **resultaten voor alle activiteiten weergeven**.</span><span class="sxs-lookup"><span data-stu-id="39e13-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="39e13-110">Klik op **zoeken**.</span><span class="sxs-lookup"><span data-stu-id="39e13-110">Click **Search**.</span></span>

<span data-ttu-id="39e13-111">Klik in de resultaten op **resultaten filteren** en **Postvak** voor typen in het vak activiteiten filter.</span><span class="sxs-lookup"><span data-stu-id="39e13-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="39e13-112">Selecteer een controlerecord in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="39e13-112">Select an audit record in the results.</span></span> <span data-ttu-id="39e13-113">Klik in het vervolgmenu **Details** op **meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="39e13-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="39e13-114">U dient de details van elke controlerecord te bekijken om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.</span><span class="sxs-lookup"><span data-stu-id="39e13-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="39e13-115">**ObjectId**: de alias waarde van het postvak dat is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="39e13-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="39e13-116">**Parameters**: _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.</span><span class="sxs-lookup"><span data-stu-id="39e13-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="39e13-117">**UserID**: de gebruiker die e-mail heeft geconfigureerd voor het postvak in het veld **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="39e13-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="39e13-118">Zie voor meer informatie [bepalen wie het doorsturen van e-mail voor een postvak heeft ingesteld](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="39e13-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
