---
title: Problemen met de eigenaar van app-registratie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404454"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="36625-102">Problemen met de eigenaar van app-registratie</span><span class="sxs-lookup"><span data-stu-id="36625-102">App Registration Owner issues</span></span>

<span data-ttu-id="36625-103">Hieronder volgen de beschikbare methoden om principals toe te voegen als eigenaren voor app-registraties:</span><span class="sxs-lookup"><span data-stu-id="36625-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="36625-104">Azure AD PowerShell-module gebruiken -</span><span class="sxs-lookup"><span data-stu-id="36625-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="36625-105">Verwijzing: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="36625-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="36625-106">Azure CLI gebruiken - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="36625-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="36625-107">Verwijzing: [eigenaar van az-ad-app](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="36625-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="36625-108">MS Graph gebruiken -</span><span class="sxs-lookup"><span data-stu-id="36625-108">Using MS Graph -</span></span>

    <span data-ttu-id="36625-109">Verwijzing: [Eigenaar toevoegen - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="36625-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="36625-110">De Azure AD Portal gebruiken: ga naar [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Selecteer uw toepassing > Eigenaren > Eigenaren toevoegen</span><span class="sxs-lookup"><span data-stu-id="36625-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="36625-111">**Kunt u uw toepassing niet weergeven op app-registraties, ook al bent u de eigenaar van die toepassing?**</span><span class="sxs-lookup"><span data-stu-id="36625-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="36625-112">Eigenaar van een app is geen administratieve rol.</span><span class="sxs-lookup"><span data-stu-id="36625-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="36625-113">Als de instelling Toegang tot Azure AD-beheerportal beperken is ingeschakeld, kan alleen de beheerder de toepassingen bekijken in de app-registratieportal. [](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions)</span><span class="sxs-lookup"><span data-stu-id="36625-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="36625-114">Als een eigenaar de toepassingen wil kunnen bekijken, schakelt u deze instelling uit (Dit instellen op NEE) of wijst u de beheerdersrol toe aan de eigenaar voor alleen de specifieke toepassing.</span><span class="sxs-lookup"><span data-stu-id="36625-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="36625-115">Hiervoor moet u echter een Azure AD Premium P2-licentie hebben en [Privileged Identity Management inschakelen.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="36625-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
