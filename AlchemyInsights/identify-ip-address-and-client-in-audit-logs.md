---
title: IP-adres en de client in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752055"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="d7d0b-102">IP-adres en de client in de controlelogboeken geïdentificeerd</span><span class="sxs-lookup"><span data-stu-id="d7d0b-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="d7d0b-103">Het IP-adres dat overeenkomt met een activiteit van een gebruiker of beheerder wordt weergegeven in de controlelogboeken.</span><span class="sxs-lookup"><span data-stu-id="d7d0b-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="d7d0b-104">Ook de informatie over de client is vastgelegd.</span><span class="sxs-lookup"><span data-stu-id="d7d0b-104">The client information is also logged.</span></span> <span data-ttu-id="d7d0b-105">Hier volgen de stappen voor het identificeren van dergelijke informatie</span><span class="sxs-lookup"><span data-stu-id="d7d0b-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="d7d0b-106">Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d7d0b-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d7d0b-107">Klik op **Zoeken en onderzoek** en **Audit-logboek zoeken**selecteren.</span><span class="sxs-lookup"><span data-stu-id="d7d0b-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="d7d0b-108">Als u geïnteresseerd in een bepaalde activiteit bent, selecteert u deze uit de lijst met **activiteiten** .</span><span class="sxs-lookup"><span data-stu-id="d7d0b-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="d7d0b-109">Niet alle activiteiten worden geretourneerd voor de geselecteerde gebruiker (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="d7d0b-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="d7d0b-110">**Opmerking**: bepaalde activiteiten zijn mogelijk niet beschikbaar in het menu **activiteiten** ; echter die items controleren wordt geretourneerd als **Resultaat voor alle activiteiten weergeven** is geselecteerd (standaard instelling).</span><span class="sxs-lookup"><span data-stu-id="d7d0b-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="d7d0b-111">Geef de gebruikersnaam op in het veld **gebruikers** , selecteert u het gewenste datumbereik voor de activiteit en klik op **Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="d7d0b-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="d7d0b-112">In de resultaten, kunt u het IP-adres voor die activiteit in het resultatendeelvenster te zien.</span><span class="sxs-lookup"><span data-stu-id="d7d0b-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="d7d0b-113">Selecteer de record audit voor gedetailleerde informatie in het doel **Details** (bijvoorbeeld Client, gebruiker uitgevoerd, actie, enz.).</span><span class="sxs-lookup"><span data-stu-id="d7d0b-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="d7d0b-114">Zie voor meer informatie, [Zoeken naar het IP-adres van de computer toegang krijgen tot een account die oneigenlijk wordt gebruikt](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="d7d0b-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
