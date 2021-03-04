---
title: Implementatie van GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427257"
---
# <a name="gpo-deployment"></a><span data-ttu-id="16038-102">Implementatie van GPO</span><span class="sxs-lookup"><span data-stu-id="16038-102">GPO Deployment</span></span>

<span data-ttu-id="16038-103">Instellingen voor gebruikers- en computerobjecten in Azure Active Directory Domain Services (Azure AD DS) worden vaak beheerd met GPOs (Group Policy Objects).</span><span class="sxs-lookup"><span data-stu-id="16038-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="16038-104">Azure AD DS bevat ingebouwde GPOs voor de AADDC-gebruikers en AADDC-computerscontainers.</span><span class="sxs-lookup"><span data-stu-id="16038-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="16038-105">U kunt deze ingebouwde GPOs aanpassen om groepsbeleid te configureren wanneer dat nodig is voor uw omgeving.</span><span class="sxs-lookup"><span data-stu-id="16038-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="16038-106">Leden van de groep Azure AD DC-beheerders hebben beheerdersbevoegdheden voor groepsbeleid in het Azure AD DS-domein en kunnen ook aangepaste GPOs- en organisatie-eenheden (OUs) maken.</span><span class="sxs-lookup"><span data-stu-id="16038-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="16038-107">Zie Overzicht van groepsbeleid voor meer informatie over wat groepsbeleid is en [hoe het werkt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="16038-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="16038-108">In een hybride omgeving worden groepsbeleidsregels die zijn geconfigureerd in een on-premises AD DS-omgeving niet gesynchroniseerd met Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="16038-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="16038-109">Als u configuratie-instellingen voor gebruikers of computers wilt definiëren in Azure AD DS, bewerkt u een van de standaard-GPOs's of maakt u een aangepast groep groep.</span><span class="sxs-lookup"><span data-stu-id="16038-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="16038-110">In dit [artikel wordt beschreven](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hoe u groepsbeleidsbeheerprogramma's installeert, hoe u de ingebouwde GPOS's bewerkt en hoe u aangepaste GPOs's maakt.</span><span class="sxs-lookup"><span data-stu-id="16038-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
