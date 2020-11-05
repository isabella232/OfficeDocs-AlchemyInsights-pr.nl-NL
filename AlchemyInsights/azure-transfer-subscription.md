---
title: Eigendom van Azure-facturering overbrengen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922031"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="b8fb6-102">Eigendom van Azure-facturering overbrengen</span><span class="sxs-lookup"><span data-stu-id="b8fb6-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="b8fb6-103">Meld u aan bij de [Azure-Portal](https://portal.azure.com/) als beheerder van het factuur account met het abonnement dat u wilt overzetten.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="b8fb6-104">Als u niet zeker weet of u een beheerder bent, of als u wilt bepalen wie dit doet, raadpleegt u de [rekening factureringsbeheerder bepalen](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="b8fb6-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="b8fb6-105">Zoek op **kostenbeheer + facturering**.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="b8fb6-106">Selecteer **abonnementen** in het linkerdeelvenster.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="b8fb6-107">Afhankelijk van de toegang moet u mogelijk een factuur bereik selecteren en vervolgens **abonnementen** of **Azure-abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="b8fb6-108">Selecteer het eigendom van de **facturering** voor het abonnement dat u wilt overzetten</span><span class="sxs-lookup"><span data-stu-id="b8fb6-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="b8fb6-109">Voer het e-mailadres in van een gebruiker die een factureringsbeheerder is van het account dat de nieuwe eigenaar wordt van het abonnement en selecteer vervolgens **overdrachtsaanvraag verzenden** .</span><span class="sxs-lookup"><span data-stu-id="b8fb6-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="b8fb6-110">De gebruiker ontvangt een e-mail met instructies om uw overdrachtsaanvraag te controleren.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="b8fb6-111">De gebruiker kan de koppeling in het e-mailbericht selecteren en de instructies volgen om de overdrachtsaanvraag goed te keuren.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="b8fb6-112">**Opmerking** : als u het eigendom van uw abonnement overdraagt naar het account van een gebruiker in een andere Azure AD-Tenant, worden alle toewijzingen met [toegangsbeheer voor rollen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)voor het beheren van resources in het abonnement blijvend verwijderd.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="b8fb6-113">Alleen de nieuwe eigenaar kan de bronnen in het abonnement beheren.</span><span class="sxs-lookup"><span data-stu-id="b8fb6-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="b8fb6-114">Zie voor meer informatie [een abonnement overzetten naar een gebruiker in een andere Azure AD-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b8fb6-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b8fb6-115">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="b8fb6-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="b8fb6-116">Facturering van een Azure-abonnement overzetten naar een ander account</span><span class="sxs-lookup"><span data-stu-id="b8fb6-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="b8fb6-117">Het eigendom van de facturering overzetten voor een Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="b8fb6-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="b8fb6-118">De overdracht van Visual Studio, Microsoft Partner Network (MPN) en betalen naar gebruik-ontwikkelaars/proefabonnementen</span><span class="sxs-lookup"><span data-stu-id="b8fb6-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="b8fb6-119">Veelgestelde vragen over het overdragen van eigendom</span><span class="sxs-lookup"><span data-stu-id="b8fb6-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="b8fb6-120">Problemen met de overdracht van eigendom oplossen</span><span class="sxs-lookup"><span data-stu-id="b8fb6-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
