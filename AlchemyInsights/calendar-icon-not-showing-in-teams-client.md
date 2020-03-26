---
title: Agendapictogram dat niet wordt weergegeven in Teams-client
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931982"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="2c0f8-102">Agendapictogram dat niet wordt weergegeven in Teams-client</span><span class="sxs-lookup"><span data-stu-id="2c0f8-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="2c0f8-103">Het tabblad Agenda in Teams vereist toegang tot een Exchange-postvak via Exchange-webservices.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="2c0f8-104">Het Exchange-postvak kan online of on-premises zijn.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="2c0f8-105">Voor online gebruikers die het tabblad Agenda niet zien, controleert u of deze [een licentie hebben voor een Exchange Online-postvak en het postvak is ingeschakeld](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2c0f8-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="2c0f8-106">Als de gebruiker een geldig postvak in Exchange Online heeft, maar het tabblad Agenda nog steeds niet wordt weergeven, ondervindt u mogelijk een netwerkprobleem.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="2c0f8-107">Gebruik de [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) en voer de **Microsoft Exchange-webservices-connectiviteitstests** uit voor de betrokken gebruiker.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="2c0f8-108">Controleer ten slotte de [Teams-apps app-beleidsinstellingen](https://admin.teams.microsoft.com/policies/app-setup) om er zeker van te zijn dat de Agenda-app niet is verwijderd uit het beleid dat op de gebruiker is toegepast (waarschijnlijk de **Wereldwijd (organisatiebreed standaard)**).</span><span class="sxs-lookup"><span data-stu-id="2c0f8-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="2c0f8-109">Als uw gebruikers on-premises zijn, moet u controleren of de hybride configuratie in orde is.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="2c0f8-110">Gebruik de [Wizard hybride configuratie](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) om problemen op te lossen.</span><span class="sxs-lookup"><span data-stu-id="2c0f8-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="2c0f8-111">Hou in het achterhoofd dat [Teams Exchange 2016 CU3 of hoger vereist](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="2c0f8-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
