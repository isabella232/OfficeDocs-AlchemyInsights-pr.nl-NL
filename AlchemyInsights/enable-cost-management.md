---
title: Kostenbeheer inschakelen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677218"
---
# <a name="enable-cost-management"></a><span data-ttu-id="7f393-102">Kostenbeheer inschakelen</span><span class="sxs-lookup"><span data-stu-id="7f393-102">Enable cost management</span></span>

<span data-ttu-id="7f393-103">**Wat betekenen de kosten voor uw organisatie?**</span><span class="sxs-lookup"><span data-stu-id="7f393-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="7f393-104">Organisaties die gebruikmaken van Enterprise Agreement (EA) of Microsoft Customer Agreement (MCA), kunnen de toegang tot kosteninformatie en prijsinformatie uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="7f393-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="7f393-105">Nadat u zich hebt aangemeld bij een Azure-Portal, kunnen ze de bewerkings-Api's van de apps gebruiken om via programmatisch een factuur te krijgen (indien aangemeld) en gebruiksinformatie.</span><span class="sxs-lookup"><span data-stu-id="7f393-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="7f393-106">**Toestaan dat extra gebruikers toegang hebben tot facturen**</span><span class="sxs-lookup"><span data-stu-id="7f393-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="7f393-107">Ga naar **blad abonnementen** in azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7f393-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="7f393-108">Selecteer **facturen** en vervolgens **toegang tot facturen**.</span><span class="sxs-lookup"><span data-stu-id="7f393-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="7f393-109">Schakel de toegang in, gevolgd door de wijzigingen op te slaan, zodat gebruikers met rollen met een abonnement kunnen facturen kunnen downloaden.</span><span class="sxs-lookup"><span data-stu-id="7f393-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="7f393-110">De account beheerder kan ook configureren dat facturen via e-mail worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="7f393-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="7f393-111">Zie [uw factuur via E-mail ontvangen](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7f393-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="7f393-112">**Gebruikers toevoegen aan de rol van facturerings lezer**</span><span class="sxs-lookup"><span data-stu-id="7f393-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="7f393-113">Ga naar **blad abonnementen** in azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7f393-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="7f393-114">Selecteer **toegangsbeheer (IAM)** en klik op **toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="7f393-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="7f393-115">Kies **facturerings lezer** op de pagina **Selecteer een rol** .</span><span class="sxs-lookup"><span data-stu-id="7f393-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="7f393-116">Typ het e-mailadres van de gebruiker die u wilt uitnodigen en klik op **OK** om de uitnodiging te verzenden.</span><span class="sxs-lookup"><span data-stu-id="7f393-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="7f393-117">Volg de instructies in de e-mail uitnodigen om u aan te melden als facturerings lezer.</span><span class="sxs-lookup"><span data-stu-id="7f393-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="7f393-118">Zie voor meer informatie de optie [toegang tot facturering verlenen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="7f393-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="7f393-119">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="7f393-119">**Recommended documents**</span></span>

- [<span data-ttu-id="7f393-120">DA-en AO-weergaven inschakelen via EA Portal</span><span class="sxs-lookup"><span data-stu-id="7f393-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="7f393-121">Kosten in kostenbeheer</span><span class="sxs-lookup"><span data-stu-id="7f393-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="7f393-122">Ondersteunde Microsoft Azure-aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="7f393-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="7f393-123">Kosten controleren in kostenanalyse</span><span class="sxs-lookup"><span data-stu-id="7f393-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="7f393-124">Toegang tot de factureringsgegevens geven</span><span class="sxs-lookup"><span data-stu-id="7f393-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="7f393-125">Toegang tot een Microsoft-klant overeenkomst controleren</span><span class="sxs-lookup"><span data-stu-id="7f393-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






