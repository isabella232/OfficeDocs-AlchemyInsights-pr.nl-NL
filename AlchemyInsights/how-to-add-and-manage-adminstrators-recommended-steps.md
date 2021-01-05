---
title: 'Beheerders toevoegen en beheren: aanbevolen stappen'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755830"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="cb7e0-102">Beheerders toevoegen en beheren: aanbevolen stappen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="cb7e0-103">Op basis van uw beschrijving van het probleem hebben we een oplossing voor u gevonden.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="cb7e0-104">De meeste klanten konden hun probleem zelf oplossen na de documentatie.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="cb7e0-105">**De beheerder of mede beheerder van het abonnement bewerken**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="cb7e0-106">De account beheerder kan beide rollen bewerken, terwijl de abonnement beheerder alleen co-beheerders in de [Azure-Portal](https://ms.portal.azure.com/#home)kan wijzigen.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="cb7e0-107">Azure-abonnements beheerders toevoegen of wijzigen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="cb7e0-108">**De abonnements beheerder of het Co-Administrator voor interne (onvoeren) abonnementen bijwerken**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="cb7e0-109">De service beheerder of de co-beheerder kan de volgende stappen uitvoeren om deze actie uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="cb7e0-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="cb7e0-110">Meld u aan bij de [Azure-Portal](https://ms.portal.azure.com/#home) en klik op **Cost Management + facturering** in het linker blad.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="cb7e0-111">Klik op het regelitem met uw abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="cb7e0-112">Hiermee opent u het overzicht voor uw abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="cb7e0-113">Klik in de Blade **abonnement** op **Eigenschappen**.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="cb7e0-114">Klik op de knop **service beheerder** .</span><span class="sxs-lookup"><span data-stu-id="cb7e0-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="cb7e0-115">Voer het e-mailadres in van de gebruiker die u als service beheerder wilt instellen en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="cb7e0-116">**Co-beheerder toevoegen/wijzigen/verwijderen**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="cb7e0-117">Meld u bij de [Azure-Portal](https://ms.portal.azure.com/#home) aan als een service beheerder.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="cb7e0-118">Open [abonnementen](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) en selecteer een abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="cb7e0-119">(Coadminstrators kan alleen worden toegewezen aan het abonnements bereik.)</span><span class="sxs-lookup"><span data-stu-id="cb7e0-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="cb7e0-120">Ga naar **toegangsbeheer (IAM)**  >  **klassieke beheerders**  >  **toevoegen**  >  **co-beheerder** toevoegen om het deelvenster **co-beheerder toevoegen** te openen (als de optie co-beheerder toevoegen is uitgeschakeld, wordt aangegeven dat u geen machtigingen hebt).</span><span class="sxs-lookup"><span data-stu-id="cb7e0-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="cb7e0-121">Selecteer de gebruiker die u wilt toevoegen en klik op **toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="cb7e0-122">**Meer informatie:**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-122">**Learn more:**</span></span>
- [<span data-ttu-id="cb7e0-123">Een co-beheerder toevoegen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="cb7e0-124">Een co-beheerder verwijderen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="cb7e0-125">De service beheerder wijzigen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="cb7e0-126">De account beheerder weergeven</span><span class="sxs-lookup"><span data-stu-id="cb7e0-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="cb7e0-127">Toegang beheren met RBAC en Azure Portal</span><span class="sxs-lookup"><span data-stu-id="cb7e0-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="cb7e0-128">**Gebruikers toevoegen/verwijderen via Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="cb7e0-129">U kunt nieuwe gebruikers toevoegen of bestaande gebruikers verwijderen uit uw Azure Active Directory-organisatie (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="cb7e0-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="cb7e0-130">Als u een nieuwe gebruiker wilt toevoegen, meldt u zich aan bij de [Azure-Portal](https://ms.portal.azure.com/#home) als gebruiker van de beheerder van de organisatie.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="cb7e0-131">Selecteer **Azure Active Directory**, selecteer **gebruikers** en klik vervolgens op **nieuwe gebruiker**.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="cb7e0-132">Vul de vereiste gegevens in op de pagina van de **gebruiker** .</span><span class="sxs-lookup"><span data-stu-id="cb7e0-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="cb7e0-133">Klik op **Maken**.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-133">Click **Create**.</span></span> <span data-ttu-id="cb7e0-134">De gebruiker wordt gemaakt en toegevoegd aan uw Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="cb7e0-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="cb7e0-135">Meer **informatie**:</span><span class="sxs-lookup"><span data-stu-id="cb7e0-135">**Learn more**:</span></span>

- [<span data-ttu-id="cb7e0-136">Een nieuwe gebruiker toevoegen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="cb7e0-137">Een gebruiker verwijderen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="cb7e0-138">Gebruikersprofielgegevens toevoegen of bijwerken met Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cb7e0-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="cb7e0-139">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="cb7e0-139">**Recommended documents**</span></span>

- [<span data-ttu-id="cb7e0-140">Wat is toegangsbeheer op basis van rollen?</span><span class="sxs-lookup"><span data-stu-id="cb7e0-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="cb7e0-141">Meer informatie over de verschillende rollen in azure</span><span class="sxs-lookup"><span data-stu-id="cb7e0-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="cb7e0-142">Machtigingen voor beheerdersrollen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cb7e0-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="cb7e0-143">Zelfstudie: toegang verlenen aan een gebruiker met behulp van RBAC en de Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="cb7e0-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="cb7e0-144">Problemen met RBAC in azure oplossen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="cb7e0-145">Uw resources organiseren met Azure-beheergroepen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="cb7e0-146">Het aanvragen van een kopie van Azure factuur via e-mail aanvragen</span><span class="sxs-lookup"><span data-stu-id="cb7e0-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="cb7e0-147">Een creditcard of betaalkaart toevoegen, bijwerken of verwijderen uit Azure</span><span class="sxs-lookup"><span data-stu-id="cb7e0-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="cb7e0-148">Het abonnement beheren (opnieuw activeren/Annuleren/activeren)</span><span class="sxs-lookup"><span data-stu-id="cb7e0-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



