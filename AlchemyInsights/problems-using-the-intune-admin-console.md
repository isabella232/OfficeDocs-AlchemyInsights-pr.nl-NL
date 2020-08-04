---
title: Problemen met het gebruik van de Intune-beheerconsole
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555036"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="4a152-102">Problemen met het gebruik van de Intune-beheerconsole</span><span class="sxs-lookup"><span data-stu-id="4a152-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="4a152-103">**'Toegang geweigerd' bij het navigeren door de Intune-beheerportal.**</span><span class="sxs-lookup"><span data-stu-id="4a152-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="4a152-104">Als u lid bent van een aangepaste Functie in Intune, moet u ervoor zorgen dat een Intune- of Enterprise Mobility Suite-licentie (EMS) aan uw account wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="4a152-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="4a152-105">Als u Configuration Manager gebruikt om apparaten te beheren, controleert u of u geen deel uitmaakt van de Intune-gebruikersverzameling voor Configuratiebeheer MDM.</span><span class="sxs-lookup"><span data-stu-id="4a152-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="4a152-106">Controleer of u de juiste RBAC-machtigingen (Role-based Administration Control) hebt gekregen in het intune-rollenblad.</span><span class="sxs-lookup"><span data-stu-id="4a152-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="4a152-107">Controleer of de gebruikte groep geen distributielijst is.</span><span class="sxs-lookup"><span data-stu-id="4a152-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="4a152-108">Intune in de Azure-portal ondersteunt alleen gebruikersaccounts die deel uitmaken van Azure Active Directory-beveiligingsgroepen.</span><span class="sxs-lookup"><span data-stu-id="4a152-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="4a152-109">Controleer uw groepen in de Azure-portal > **Intune-groepen**  >  **Groups**of in Azure-portal > Azure **Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="4a152-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="4a152-110">**Gebruiker heeft te veel machtigingen voor toegewezen Intune-rol**</span><span class="sxs-lookup"><span data-stu-id="4a152-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="4a152-111">Adviseer de gebruiker om naar **Intune**  >  **Intune-rollen**te gaan  >  **Mijn machtigingen**  >  **exporteren** om verleende machtigingen te controleren.</span><span class="sxs-lookup"><span data-stu-id="4a152-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="4a152-112">**Ik heb een scopegroep aan een rol toegevoegd, maar gebruikers in die rol zien nog steeds andere gebruikers of apparaten.**</span><span class="sxs-lookup"><span data-stu-id="4a152-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="4a152-113">Scopegroepen filteren geen gebruikers of apparaten uit.</span><span class="sxs-lookup"><span data-stu-id="4a152-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="4a152-114">Scopegroepen:</span><span class="sxs-lookup"><span data-stu-id="4a152-114">Scope groups:</span></span>

- <span data-ttu-id="4a152-115">Beperk aan wie gebruikers beleid of toepassingen kunnen toewijzen.</span><span class="sxs-lookup"><span data-stu-id="4a152-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="4a152-116">Sta alleen specifieke gebruikers toe om externe taken uit te voeren op apparaten.</span><span class="sxs-lookup"><span data-stu-id="4a152-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="4a152-117">Zie [Role-based access control (RBAC) met Microsoft Intune voor](https://docs.microsoft.com/intune/role-based-access-control)meer informatie over scopegroepen.</span><span class="sxs-lookup"><span data-stu-id="4a152-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4a152-118">**Ik heb een gebruiker toegevoegd aan een Intune-rol, maar ze hebben nog steeds volledige toegang tot de Intune-beheerconsole.**</span><span class="sxs-lookup"><span data-stu-id="4a152-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="4a152-119">Navigeer naar Intune > **Gebruikers** in de Azure-portal en controleer of de gebruiker niet is toegewezen aan een van de volgende rollen in de Azure-portal:</span><span class="sxs-lookup"><span data-stu-id="4a152-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="4a152-120">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="4a152-120">Global administrator</span></span>
- <span data-ttu-id="4a152-121">Intune-servicebeheerder</span><span class="sxs-lookup"><span data-stu-id="4a152-121">Intune service administrator</span></span>
- <span data-ttu-id="4a152-122">SharePoint-beheerder</span><span class="sxs-lookup"><span data-stu-id="4a152-122">SharePoint administrator</span></span>

<span data-ttu-id="4a152-123">Zie [Role-based access control (RBAC) met Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4a152-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4a152-124">**Toegangsproblemen**</span><span class="sxs-lookup"><span data-stu-id="4a152-124">**Access Issues**</span></span>

<span data-ttu-id="4a152-125">Zie [U zich niet aanmelden bij Office 365, Azure of Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4a152-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>