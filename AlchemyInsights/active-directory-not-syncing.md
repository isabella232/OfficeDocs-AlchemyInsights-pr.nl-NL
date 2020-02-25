---
title: Active Directory synchroniseert niet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265156"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="2d63b-102">Active Directory synchroniseert niet</span><span class="sxs-lookup"><span data-stu-id="2d63b-102">Active Directory not syncing</span></span>

<span data-ttu-id="2d63b-103">Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie' of de status van adreslijstsynchronisatie in de Office-beheerportal opmerkt: 'Laatst gesynchroniseerd meer dan 3 dagen geleden', kan het zijn dat AADConnect onjuiste instellingen of onvoldoende heeft machtigingen om een synchronisatie uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="2d63b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="2d63b-104">Het opnieuw installeren van AADConnect met behulp van expresinstellingen kan het probleem snel oplossen:</span><span class="sxs-lookup"><span data-stu-id="2d63b-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="2d63b-105">[Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="2d63b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="2d63b-106">[Volg de instructies voor express installatie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="2d63b-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="2d63b-107">Zie [Azure AD Connect: Accounts en machtigingen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.</span><span class="sxs-lookup"><span data-stu-id="2d63b-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
