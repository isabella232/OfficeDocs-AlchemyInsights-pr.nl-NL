---
title: Het IP-adres zoeken in het auditlogboek
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481722"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="34220-102">Het IP-adres zoeken in het auditlogboek</span><span class="sxs-lookup"><span data-stu-id="34220-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="34220-103">Het IP-adres dat overeenkomt met een activiteit die is uitgevoerd door een gebruiker of beheerder, wordt weergegeven in de auditlogboeken.</span><span class="sxs-lookup"><span data-stu-id="34220-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="34220-104">De klantgegevens worden ook in het logbestand vastgelegd.</span><span class="sxs-lookup"><span data-stu-id="34220-104">The client information is also logged.</span></span> <span data-ttu-id="34220-105">U kunt als volgende informatie het IP-adres identificeren:</span><span class="sxs-lookup"><span data-stu-id="34220-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="34220-106">Ga naar het [Office 365-& compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="34220-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="34220-107">Selecteer **Zoeken in**  >  **[auditlogboek zoeken.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="34220-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="34220-108">Als u een melding ziet dat u de controle moet in- of uitvoeren, gaat u door en schakel deze nu in.</span><span class="sxs-lookup"><span data-stu-id="34220-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="34220-109">Als deze functie niet is ingeschakeld, kunnen er geen gegevens worden verzameld uit eerdere datums.</span><span class="sxs-lookup"><span data-stu-id="34220-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="34220-110">Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in de **lijst Activiteiten.** anders worden standaard alle activiteiten geretourneerd voor de geselecteerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="34220-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="34220-111">Bepaalde activiteiten zijn mogelijk niet beschikbaar voor selectie in **het** menu Activiteiten. Deze controle-items worden echter wel geretourneerd als Resultaten tonen voor **alle** activiteiten is geselecteerd (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="34220-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="34220-112">Geef het datumbereik op en selecteer in het veld **Gebruikers** de gebruikersnaam voor de gebruiker die u wilt onderzoeken.</span><span class="sxs-lookup"><span data-stu-id="34220-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="34220-113">Selecteer **Zoeken.**</span><span class="sxs-lookup"><span data-stu-id="34220-113">Select **Search**.</span></span> <span data-ttu-id="34220-114">De activiteiten worden weergegeven onder **Resultaten.**</span><span class="sxs-lookup"><span data-stu-id="34220-114">The activities appear under **Results**.</span></span> <span data-ttu-id="34220-115">U kunt het IP-adres voor elke activiteit zien.</span><span class="sxs-lookup"><span data-stu-id="34220-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="34220-116">Als u details wilt weergeven, selecteert u een activiteit en vervolgens **Meer informatie.**</span><span class="sxs-lookup"><span data-stu-id="34220-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="34220-117">Zie Het Auditlogboek van Office 365 doorzoeken voor meer informatie [om veelvoorkomende scenario's op te lossen.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="34220-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>