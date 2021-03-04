---
title: Ontdek wie doorsturen heeft ingesteld voor een postvak en hoe
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429419"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="9a36b-102">Ontdek wie doorsturen heeft ingesteld voor een postvak en hoe</span><span class="sxs-lookup"><span data-stu-id="9a36b-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="9a36b-103">Als extern doorsturen is ingesteld voor een postvak, wordt de activiteit gecontroleerd als onderdeel van de Set-Mailbox-cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9a36b-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="9a36b-104">U kunt de activiteit als volgen vinden in het auditlogboek:</span><span class="sxs-lookup"><span data-stu-id="9a36b-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="9a36b-105">Ga naar het [Office 365-& compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="9a36b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="9a36b-106">Selecteer **Zoeken in** >  **auditlogboek zoeken.**</span><span class="sxs-lookup"><span data-stu-id="9a36b-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="9a36b-107">Als u een melding ziet dat u de controle moet in- of uitvoeren, gaat u door en schakel deze nu in.</span><span class="sxs-lookup"><span data-stu-id="9a36b-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="9a36b-108">Als deze functie niet is ingeschakeld, kunnen er geen gegevens worden verzameld uit eerdere datums.</span><span class="sxs-lookup"><span data-stu-id="9a36b-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="9a36b-109">Zorg ervoor dat **het veld** Activiteiten is ingesteld op Resultaten tonen voor **alle activiteiten** (de standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="9a36b-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="9a36b-110">Geef het datumbereik op.</span><span class="sxs-lookup"><span data-stu-id="9a36b-110">Specify the date range.</span></span> <span data-ttu-id="9a36b-111">U hoeft geen gebruikersnaam op te geven.</span><span class="sxs-lookup"><span data-stu-id="9a36b-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="9a36b-112">Selecteer **Zoeken.**</span><span class="sxs-lookup"><span data-stu-id="9a36b-112">Select **Search**.</span></span> <span data-ttu-id="9a36b-113">De activiteiten worden weergegeven onder **Resultaten.**</span><span class="sxs-lookup"><span data-stu-id="9a36b-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="9a36b-114">Selecteer **Filterresultaten** en typ **Postvak Instellen** in het **veld Activiteitsfilter.**</span><span class="sxs-lookup"><span data-stu-id="9a36b-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="9a36b-115">Hiermee worden alle activiteiten **van Set-Mailbox** als retourneert.</span><span class="sxs-lookup"><span data-stu-id="9a36b-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="9a36b-116">Als u de details wilt weergeven, selecteert u een activiteit en vervolgens **Meer informatie.**</span><span class="sxs-lookup"><span data-stu-id="9a36b-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="9a36b-117">Onder **Parameters** ziet u het doorsturende e-mailadres dat is ingesteld voor het postvak.</span><span class="sxs-lookup"><span data-stu-id="9a36b-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="9a36b-118">De **UserID** vertegenwoordigt de gebruiker die extern doorsturen heeft ingesteld voor het postvak.</span><span class="sxs-lookup"><span data-stu-id="9a36b-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="9a36b-119">Zie Het Auditlogboek van Office 365 doorzoeken voor meer informatie [om veelvoorkomende scenario's op te lossen.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="9a36b-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>