---
title: De auditlogboeken voor verwijderde gebeurtenissen lezen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429372"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="990c4-102">De auditlogboeken voor verwijderde gebeurtenissen lezen</span><span class="sxs-lookup"><span data-stu-id="990c4-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="990c4-103">Dit doet u als volgende:</span><span class="sxs-lookup"><span data-stu-id="990c4-103">Here's how to do this:</span></span>

1. <span data-ttu-id="990c4-104">Ga naar het [Office 365-& compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="990c4-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="990c4-105">Selecteer **Zoeken in**  >  [**auditlogboek zoeken.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="990c4-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="990c4-106">Als u een melding ziet dat u de functie moet in- of uit moet zetten, kunt u de functie nu in- of in gang zetten.</span><span class="sxs-lookup"><span data-stu-id="990c4-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="990c4-107">Als de functie niet is ingeschakeld, kunnen er geen gegevens worden verzameld uit eerdere datums.</span><span class="sxs-lookup"><span data-stu-id="990c4-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="990c4-108">Selecteer **Activiteiten en** zoek exchange-postvakactiviteiten. </span><span class="sxs-lookup"><span data-stu-id="990c4-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="990c4-109">Selecteer de **opties Verwijderde berichten in de** map Verwijderde items en Verplaatste berichten naar **Map** Verwijderde items.</span><span class="sxs-lookup"><span data-stu-id="990c4-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="990c4-110">Wanneer u klaar bent, klikt u buiten het deelvenster om het deelvenster **Activiteiten te** minimaliseren.</span><span class="sxs-lookup"><span data-stu-id="990c4-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="990c4-111">Geef het datumbereik op en selecteer vervolgens in het vak **Gebruikers** de gebruikersnaam voor de gebruiker die u wilt onderzoeken.</span><span class="sxs-lookup"><span data-stu-id="990c4-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="990c4-112">U kunt meerdere gebruikers tegelijk selecteren.</span><span class="sxs-lookup"><span data-stu-id="990c4-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="990c4-113">Selecteer **Zoeken.**</span><span class="sxs-lookup"><span data-stu-id="990c4-113">Select **Search**.</span></span> <span data-ttu-id="990c4-114">De activiteiten worden weergegeven onder **Resultaten.**</span><span class="sxs-lookup"><span data-stu-id="990c4-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="990c4-115">Als u de details wilt weergeven, selecteert u een activiteit en vervolgens **Meer informatie.**</span><span class="sxs-lookup"><span data-stu-id="990c4-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="990c4-116">Aanvullende informatie over het verwijderde item, zoals het onderwerp en de locatie van het item toen het werd verwijderd, wordt weergegeven in het veld **Beïnvloede** Items.</span><span class="sxs-lookup"><span data-stu-id="990c4-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="990c4-117">U kunt verwijderde items niet herstellen met behulp van de functie Auditlogboek.</span><span class="sxs-lookup"><span data-stu-id="990c4-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="990c4-118">Zie Verwijderde items of e-mail herstellen in Outlook Web App als u [verwijderde items wilt herstellen.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="990c4-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="990c4-119">Zie Het Auditlogboek van Office 365 doorzoeken voor meer informatie [om veelvoorkomende scenario's op te lossen.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="990c4-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
