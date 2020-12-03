---
title: Tenant verwijderen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564486"
---
# <a name="delete-tenant"></a><span data-ttu-id="aba87-102">Tenant verwijderen</span><span class="sxs-lookup"><span data-stu-id="aba87-102">Delete tenant</span></span>

<span data-ttu-id="aba87-103">Als u een Azure AD wilt verwijderen, moet u het volgende doen:</span><span class="sxs-lookup"><span data-stu-id="aba87-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="aba87-104">U bent een globale beheerder voor de adreslijst.</span><span class="sxs-lookup"><span data-stu-id="aba87-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="aba87-105">U bent niet aangemeld met een account dat de standaardmap bevat, zoals contoso.onmicrosoft.com, in het aangemelde account, zoals admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="aba87-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="aba87-106">Verwijder actieve toepassingen in de Directory voordat u ze verwijdert.</span><span class="sxs-lookup"><span data-stu-id="aba87-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="aba87-107">Als u actieve toepassingen wilt verwijderen, gaat u naar app-registraties en verwijdert u de bestaande toepassingen.</span><span class="sxs-lookup"><span data-stu-id="aba87-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="aba87-108">Er zijn geen actieve abonnementen voor Microsoft Online Services, zoals Microsoft Azure, Office 365 of Azure AD Premium die zijn gekoppeld aan de adreslijst.</span><span class="sxs-lookup"><span data-stu-id="aba87-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="aba87-109">Verbind uw abonnementen of beëindig het annuleren van actieve abonnementen via Azure support en facturering.</span><span class="sxs-lookup"><span data-stu-id="aba87-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="aba87-110">Meer informatie over het annuleren van Office 365-en Azure-abonnementen.</span><span class="sxs-lookup"><span data-stu-id="aba87-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="aba87-111">Zie [een Azure-abonnement aan uw Azure AD-Tenant koppelen of toevoegen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)voor meer informatie over het koppelen of toevoegen van een bestaand abonnement aan een Tenant.</span><span class="sxs-lookup"><span data-stu-id="aba87-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="aba87-112">Er is geen actieve licentie.</span><span class="sxs-lookup"><span data-stu-id="aba87-112">There are no Active license.</span></span> <span data-ttu-id="aba87-113">Zie een [abonnement verwijderen om de licentie te verwijderen voor informatie over het](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)verwijderen van licenties.</span><span class="sxs-lookup"><span data-stu-id="aba87-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="aba87-114">Er zijn geen andere actieve gebruikers in de adreslijst, naast uzelf als de globale beheerder, wanneer ze probeert Azure AD te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="aba87-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="aba87-115">Verwijder andere actieve gebruikers en afhankelijkheden van een aangepaste domeinnaam in de Tenant, moet u deze ook verwijderen, zoals gebruikers die zijn gemaakt met admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="aba87-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="aba87-116">Voor meer gedetailleerde stappen voor:</span><span class="sxs-lookup"><span data-stu-id="aba87-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="aba87-117">Verwijder ' Azure Active Directory ' of ' abonnement ' en Zie [Azure Active Directory verwijderen](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="aba87-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="aba87-118">Als u toepassingen verwijdert uit de adreslijst, raadpleegt u [toepassingen verwijderen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="aba87-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
