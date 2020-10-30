---
title: Toegang tot het abonnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807292"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="5cf53-102">U kunt zich niet aanmelden bij Azure vanwege browser problemen (browser loopt vast, houdt geen spind, wordt niet geladen, etc.)</span><span class="sxs-lookup"><span data-stu-id="5cf53-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="5cf53-103">U wordt mogelijk beïnvloed door een onderbreking.</span><span class="sxs-lookup"><span data-stu-id="5cf53-103">You might be impacted by an outage.</span></span> <span data-ttu-id="5cf53-104">Kijk of er een voortdurende onderbreking is: de status van [Azure-integriteit](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="5cf53-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="5cf53-105">Meld u af bij alle actieve Azure-sessies.</span><span class="sxs-lookup"><span data-stu-id="5cf53-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="5cf53-106">Maak een privé-of Incognito-modus van uw webbrowser.</span><span class="sxs-lookup"><span data-stu-id="5cf53-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="5cf53-107">U kunt ook proberen om een browser te vernieuwen, een andere browser te gebruiken en cache cookies te verwijderen als hierboven niet werkt.</span><span class="sxs-lookup"><span data-stu-id="5cf53-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="5cf53-108">Meer informatie: [problemen met aanmelden oplossen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="5cf53-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="5cf53-109">**Geen toegang tot abonnementen**</span><span class="sxs-lookup"><span data-stu-id="5cf53-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="5cf53-110">Zorg er in de [Azure-Portal](https://portal.azure.com/)voor dat de juiste Azure-Directory is geselecteerd in het account rechtsboven.</span><span class="sxs-lookup"><span data-stu-id="5cf53-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="5cf53-111">Zorg er in het [Azure-account centrum](https://account.windowsazure.com/Subscriptions)voor dat het account dat wordt gebruikt, de accountbeheerder is.</span><span class="sxs-lookup"><span data-stu-id="5cf53-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="5cf53-112">Meer informatie: [problemen met geen abonnement gevonden](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="5cf53-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="5cf53-113">**Geen toegang tot de factureringsgeschiedenis**</span><span class="sxs-lookup"><span data-stu-id="5cf53-113">**Unable to access billing history**</span></span>

<span data-ttu-id="5cf53-114">De accountbeheerder moet ervoor zorgen dat de gebruiker die de factureringsgegevens opent, wordt toegevoegd aan Azure Active Directory als gastgebruiker: [een nieuwe gebruiker toevoegen of verwijderen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5cf53-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5cf53-115">De gebruiker moet een globale beheerdersrol krijgen: [rollen aan gebruikers toewijzen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5cf53-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5cf53-116">Plaats dit, de gebruiker kan facturerings toegang krijgen met behulp van rac's: [toegang tot facturering verlenen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5cf53-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5cf53-117">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="5cf53-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="5cf53-118">Ik kan me niet aanmelden om mijn Azure-abonnement te beheren</span><span class="sxs-lookup"><span data-stu-id="5cf53-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)