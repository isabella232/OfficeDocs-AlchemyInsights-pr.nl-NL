---
title: IP-adres en client identificeren in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508911"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="5fa25-102">IP-adres en client identificeren in controlelogboeken</span><span class="sxs-lookup"><span data-stu-id="5fa25-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="5fa25-103">Het IP-adres dat overeenkomt met een activiteit van een Microsoft 365-gebruiker of -beheerder wordt weergegeven in de controlelogboeken.</span><span class="sxs-lookup"><span data-stu-id="5fa25-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="5fa25-104">De klantgegevens worden ook geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="5fa25-104">The client information is also logged.</span></span> <span data-ttu-id="5fa25-105">Hier volgen de stappen om dergelijke informatie te identificeren</span><span class="sxs-lookup"><span data-stu-id="5fa25-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="5fa25-106">Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5fa25-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5fa25-107">Ga naar de zoekpagina **van het**  >  **zoekcontrolelogboek.**</span><span class="sxs-lookup"><span data-stu-id="5fa25-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="5fa25-108">Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in **de lijst Activiteiten.**</span><span class="sxs-lookup"><span data-stu-id="5fa25-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="5fa25-109">Als dit niet het gaat, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="5fa25-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="5fa25-110">**Opmerking**: Bepaalde activiteiten zijn mogelijk niet beschikbaar in het **menu Activiteiten;** Deze controle-items worden echter geretourneerd als **Resultaten weergeven voor alle activiteiten** is geselecteerd (standaardinstelling).</span><span class="sxs-lookup"><span data-stu-id="5fa25-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="5fa25-111">Geef de gebruikersnaam op in het veld **Gebruikers,** selecteer het juiste datumbereik voor de activiteit en klik op **Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="5fa25-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="5fa25-112">In de resultaten u het IP-adres voor die activiteit zien in het resultatenvenster.</span><span class="sxs-lookup"><span data-stu-id="5fa25-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="5fa25-113">Selecteer de controlerecord om gedetailleerde informatie te zien in de flyout **Details** (bijvoorbeeld Client, Gebruiker die actie heeft uitgevoerd, enz.).</span><span class="sxs-lookup"><span data-stu-id="5fa25-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="5fa25-114">Zie [Het IP-adres van de computer zoeken dat wordt gebruikt om toegang te krijgen tot een gecompromitteerd account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5fa25-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
