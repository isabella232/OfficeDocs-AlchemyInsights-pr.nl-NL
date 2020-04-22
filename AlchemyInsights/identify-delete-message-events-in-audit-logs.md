---
title: Berichtengebeurtenissen verwijderen in controlelogboeken identificeren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716491"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="1d44c-102">Controlelogboeken voor verwijderde e-mailberichten</span><span class="sxs-lookup"><span data-stu-id="1d44c-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="1d44c-103">Vanaf januari 2019 schakelt Microsoft standaard de controlelogboekregistratie van het postvak in.</span><span class="sxs-lookup"><span data-stu-id="1d44c-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="1d44c-104">Als u anders berichtgebeurtenissen voor een specifieke gebruiker wilt controleren, moet u de verwijderingsacties handmatig inschakelen voor controle.</span><span class="sxs-lookup"><span data-stu-id="1d44c-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="1d44c-105">Als de controlelogboekregistratie voor postvakcontroles al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, voert u de onderstaande stappen uit.</span><span class="sxs-lookup"><span data-stu-id="1d44c-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="1d44c-106">Inloggen bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1d44c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1d44c-107">Klik **op Zoeken en onderzoeken** en selecteer Zoeken in het **controlelogboek**.</span><span class="sxs-lookup"><span data-stu-id="1d44c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1d44c-108">Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.**</span><span class="sxs-lookup"><span data-stu-id="1d44c-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1d44c-109">Geef de gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd).</span><span class="sxs-lookup"><span data-stu-id="1d44c-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="1d44c-110">Selecteer in het veld **Activiteiten** de optie **Verwijderde berichten uit de map Verwijderde items** en Berichten verplaatst naar de map Verwijderde **items**.</span><span class="sxs-lookup"><span data-stu-id="1d44c-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="1d44c-111">Klik **op Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="1d44c-111">Click **Search**.</span></span>

<span data-ttu-id="1d44c-112">Selecteer in de resultaten een controlerecord.</span><span class="sxs-lookup"><span data-stu-id="1d44c-112">In the results, select an audit record.</span></span> <span data-ttu-id="1d44c-113">Klik in de flyout met details op **Meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="1d44c-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1d44c-114">Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item toen het werd verwijderd) wordt weergegeven in het veld **Getroffen Items.**</span><span class="sxs-lookup"><span data-stu-id="1d44c-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="1d44c-115">In de eigenschap **ClientInfoString** wordt weergegeven of de verwijdering heeft plaatsgevonden in Outlook, de webversie van Outlook (voorheen Outlook Web App) of een ander apparaat.</span><span class="sxs-lookup"><span data-stu-id="1d44c-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="1d44c-116">Zie [Bepalen wie e-mail doorsturen voor een postvak heeft ingesteld voor](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1d44c-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="1d44c-117">**Opmerking:** U verwijderde items niet ophalen met de functie controlelogboek.</span><span class="sxs-lookup"><span data-stu-id="1d44c-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="1d44c-118">Zie Verwijderde items herstellen [in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)als u verwijderde berichten wilt ophalen in de webversie van Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d44c-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
