---
title: Active Directory wordt niet gesynchroniseerd
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822846"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="b3c0e-102">Active Directory wordt niet gesynchroniseerd</span><span class="sxs-lookup"><span data-stu-id="b3c0e-102">Active Directory not syncing</span></span>

<span data-ttu-id="b3c0e-103">Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie', of de adreslijstsynchronisatiestatus in de Office-beheerportal 'Laatst gesynchroniseerd meer dan 3 dagen geleden' ziet, kan het zijn dat AADConnect onjuiste instellingen of onvoldoende machtigingen heeft om een synchronisatie uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="b3c0e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="b3c0e-104">Als u AADConnect opnieuw installeert met behulp van express-instellingen, kan het probleem snel worden opgelost:</span><span class="sxs-lookup"><span data-stu-id="b3c0e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="b3c0e-105">[Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="b3c0e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="b3c0e-106">[Volg de instructies voor het snel installeren.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="b3c0e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="b3c0e-107">Zie [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.</span><span class="sxs-lookup"><span data-stu-id="b3c0e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
