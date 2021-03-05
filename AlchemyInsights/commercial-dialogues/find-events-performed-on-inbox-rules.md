---
title: Gebeurtenissen zoeken die zijn uitgevoerd met regels voor Postvak IN
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481715"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="84a0e-102">Gebeurtenissen zoeken die zijn uitgevoerd met regels voor Postvak IN</span><span class="sxs-lookup"><span data-stu-id="84a0e-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="84a0e-103">Wanneer regels voor Postvak IN worden gemaakt, gewijzigd of verwijderd, worden de gebeurtenissen vastgelegd in het auditlogboek.</span><span class="sxs-lookup"><span data-stu-id="84a0e-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="84a0e-104">U kunt ze als volgende bekijken:</span><span class="sxs-lookup"><span data-stu-id="84a0e-104">Here's how to review them:</span></span>

1. <span data-ttu-id="84a0e-105">Ga naar het [Office 365-& compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="84a0e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="84a0e-106">Selecteer Zoeken > zoeken in het auditlogboek.</span><span class="sxs-lookup"><span data-stu-id="84a0e-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="84a0e-107">Als u een melding ziet dat u de controle moet in- of uitvoeren, gaat u door en schakel deze nu in.</span><span class="sxs-lookup"><span data-stu-id="84a0e-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="84a0e-108">Als deze functie niet is ingeschakeld, kunnen er geen gegevens worden verzameld uit eerdere datums.</span><span class="sxs-lookup"><span data-stu-id="84a0e-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="84a0e-109">Selecteer het veld Activiteiten, zoek Exchange-postvakactiviteiten en selecteer vervolgens New-InboxRule Regel voor Postvak IN maken in Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="84a0e-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="84a0e-110">Wanneer u klaar bent, klikt u buiten het deelvenster om het deelvenster Activiteiten te minimaliseren.</span><span class="sxs-lookup"><span data-stu-id="84a0e-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="84a0e-111">Geef het datumbereik op en selecteer vervolgens in het veld Gebruikers de gebruikersnaam voor de gebruiker die u wilt onderzoeken.</span><span class="sxs-lookup"><span data-stu-id="84a0e-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="84a0e-112">U kunt meerdere gebruikers tegelijk selecteren.</span><span class="sxs-lookup"><span data-stu-id="84a0e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="84a0e-113">Selecteer Zoeken.</span><span class="sxs-lookup"><span data-stu-id="84a0e-113">Select Search.</span></span> <span data-ttu-id="84a0e-114">De activiteiten worden weergegeven onder Resultaten.</span><span class="sxs-lookup"><span data-stu-id="84a0e-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="84a0e-115">Als u details wilt weergeven, selecteert u een activiteit en vervolgens Meer informatie.</span><span class="sxs-lookup"><span data-stu-id="84a0e-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="84a0e-116">Onder de sectie Parameters ziet u de naam van de regel, de voorwaardenset en de acties die door de regel worden ondernomen.</span><span class="sxs-lookup"><span data-stu-id="84a0e-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="84a0e-117">Zie Het auditlogboek van Office 365 doorzoeken om veelvoorkomende scenario's op te lossen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="84a0e-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>