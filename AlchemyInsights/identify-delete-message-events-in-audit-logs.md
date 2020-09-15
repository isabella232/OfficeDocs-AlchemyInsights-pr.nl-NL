---
title: Berichten verwijderen uit de logboekgebeurtenissen in auditlogboeken
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696508"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="d7233-102">Controlelogboeken voor verwijderde e-mailberichten</span><span class="sxs-lookup"><span data-stu-id="d7233-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="d7233-103">Vanaf januari 2019 wordt in Microsoft de auditlogboek registratie voor Postvak in standaard ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d7233-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="d7233-104">Als u de berichten voor een bepaalde gebruiker ook wilt verwijderen, moet u de Delete-acties handmatig inschakelen voor de controle.</span><span class="sxs-lookup"><span data-stu-id="d7233-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="d7233-105">Voer de onderstaande stappen uit als controlelogboeken voor de Postvak al zijn ingeschakeld voor uw organisatie of voor de specifieke gebruiker.</span><span class="sxs-lookup"><span data-stu-id="d7233-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="d7233-106">Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d7233-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d7233-107">Klik op **zoeken en onderzoeken** en selecteer **Zoeken in audit logboek**.</span><span class="sxs-lookup"><span data-stu-id="d7233-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d7233-108">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="d7233-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d7233-109">Geef de gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd).</span><span class="sxs-lookup"><span data-stu-id="d7233-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="d7233-110">Selecteer in het veld **activiteiten** de optie **Verwijderde berichten uit de map Verwijderde items** en **verplaatste berichten naar de map Verwijderde items**.</span><span class="sxs-lookup"><span data-stu-id="d7233-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="d7233-111">Klik op **zoeken**.</span><span class="sxs-lookup"><span data-stu-id="d7233-111">Click **Search**.</span></span>

<span data-ttu-id="d7233-112">Selecteer een controlerecord in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="d7233-112">In the results, select an audit record.</span></span> <span data-ttu-id="d7233-113">Klik in het vervolgmenu Details op **meer informatie**.</span><span class="sxs-lookup"><span data-stu-id="d7233-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d7233-114">Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item na verwijdering) wordt weergegeven in het veld **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="d7233-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="d7233-115">De eigenschap **ClientInfoString** wordt weergegeven als de verwijdering is uitgevoerd in Outlook, de webversie van Outlook (voorheen Outlook Web app) of een ander apparaat.</span><span class="sxs-lookup"><span data-stu-id="d7233-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="d7233-116">Zie voor meer informatie [bepalen wie het doorsturen van e-mail voor een postvak heeft ingesteld](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="d7233-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="d7233-117">**Opmerking**: u kunt verwijderde items niet ophalen met de functie auditlogboek.</span><span class="sxs-lookup"><span data-stu-id="d7233-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="d7233-118">Zie [Verwijderde items herstellen in Outlook Web app](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)voor informatie over het ophalen van verwijderde berichten in de webversie van Outlook.</span><span class="sxs-lookup"><span data-stu-id="d7233-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
