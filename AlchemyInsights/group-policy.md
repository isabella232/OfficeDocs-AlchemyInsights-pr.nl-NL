---
title: Groepsbeleid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256713"
---
# <a name="group-policy"></a><span data-ttu-id="3590e-102">Groepsbeleid</span><span class="sxs-lookup"><span data-stu-id="3590e-102">Group policy</span></span>

<span data-ttu-id="3590e-103">Instellingen voor gebruikers- en computerobjecten in Azure Active Directory Domain Services (Azure AD DS) worden vaak beheerd met GPOs (Group Policy Objects).</span><span class="sxs-lookup"><span data-stu-id="3590e-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="3590e-104">Azure AD DS bevat ingebouwde GPOs voor de AADDC-gebruikers en AADDC-computerscontainers.</span><span class="sxs-lookup"><span data-stu-id="3590e-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="3590e-105">U kunt deze ingebouwde GPOs aanpassen om groepsbeleid te configureren wanneer dat nodig is voor uw omgeving.</span><span class="sxs-lookup"><span data-stu-id="3590e-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="3590e-106">Leden van de beheerdersgroep Azure AD DC hebben bevoegdheden voor groepsbeleidsbeheer in het Azure AD DS-domein en kunnen ook aangepaste GPOs- en organisatie-eenheden (OUs) maken.</span><span class="sxs-lookup"><span data-stu-id="3590e-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="3590e-107">Zie overzicht van groepsbeleid voor meer informatie over wat groepsbeleid is en [hoe dit werkt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="3590e-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="3590e-108">In een hybride omgeving worden groepsbeleidsregels die zijn geconfigureerd in een on-premises AD DS-omgeving niet gesynchroniseerd met Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="3590e-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="3590e-109">Als u configuratie-instellingen voor gebruikers of computers wilt definiëren in Azure AD DS, bewerkt u een van de standaard-GPOs's of maakt u een aangepast groep groep.</span><span class="sxs-lookup"><span data-stu-id="3590e-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="3590e-110">In dit [artikel wordt beschreven](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hoe u groepsbeleidsbeheerprogramma's installeert, hoe u de ingebouwde GPOS's bewerkt en hoe u aangepaste GPOs's maakt.</span><span class="sxs-lookup"><span data-stu-id="3590e-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



