---
title: IP-adres en de client identificeren in controlelogboeken
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668305"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8748d-102">IP-adres en de client identificeren in controlelogboeken</span><span class="sxs-lookup"><span data-stu-id="8748d-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8748d-103">Het IP-adres dat overeenkomt met een activiteit door een Microsoft 365-gebruiker of-beheerder, wordt weergegeven in de controlelogboeken.</span><span class="sxs-lookup"><span data-stu-id="8748d-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8748d-104">De clientinformatie wordt ook vastgelegd.</span><span class="sxs-lookup"><span data-stu-id="8748d-104">The client information is also logged.</span></span> <span data-ttu-id="8748d-105">Dit zijn de stappen voor het identificeren van deze informatie:</span><span class="sxs-lookup"><span data-stu-id="8748d-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8748d-106">Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="8748d-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="8748d-107">Ga **naar de pagina zoeken in**het  >  **audit logboek** .</span><span class="sxs-lookup"><span data-stu-id="8748d-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="8748d-108">Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in de lijst **activiteiten** .</span><span class="sxs-lookup"><span data-stu-id="8748d-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8748d-109">Als dat niet zo is, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="8748d-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8748d-110">**Opmerking**: in het **activiteiten** menu zijn bepaalde activiteiten mogelijk niet beschikbaar. deze controle items worden echter als resultaat gegeven als de optie **resultaten voor alle activiteiten weergeven** is geselecteerd (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="8748d-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8748d-111">Geef in het veld **gebruikers** de gebruikersnaam op, selecteer het juiste datumbereik voor de activiteit en klik vervolgens op **zoeken**.</span><span class="sxs-lookup"><span data-stu-id="8748d-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8748d-112">In de resultaten ziet u het IP-adres van de activiteit in het deelvenster resultaten.</span><span class="sxs-lookup"><span data-stu-id="8748d-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8748d-113">Selecteer de controlerecord om gedetailleerde informatie weer te geven in het vervolgmenu **Details** (bijvoorbeeld klant, gebruiker die actie heeft uitgevoerd, enzovoort).</span><span class="sxs-lookup"><span data-stu-id="8748d-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8748d-114">Zie voor meer informatie [het IP-adres van de computer die wordt gebruikt om toegang te krijgen tot een gemanipuleerd account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="8748d-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
