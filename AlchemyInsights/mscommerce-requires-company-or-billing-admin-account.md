---
title: Verbinding maken met de MSCommerce-module
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 10ef2e8fa7c564d53177a52136eb48cd709e5c55
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158493"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="8f85e-102">MSCommerce vereist een account voor bedrijfs- of factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="8f85e-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="8f85e-103">De MSCommerce-module vereist een account met de bevoegdheden van bedrijfs- of factureringsbeheerder.</span><span class="sxs-lookup"><span data-stu-id="8f85e-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="8f85e-104">Als u de volgende fout ontvangt, moet u opnieuw verbinding maken met een ander account.</span><span class="sxs-lookup"><span data-stu-id="8f85e-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="8f85e-105">*ErrorMessage - De externe server heeft een fout geretourneerd: (403) Verboden. Foutgegevens - Bij C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="8f85e-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="8f85e-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Kan niet opnieuw ...*</span><span class="sxs-lookup"><span data-stu-id="8f85e-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="8f85e-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="8f85e-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="8f85e-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : Niet gespecificeerd: (:) [Schrijffout], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="8f85e-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="8f85e-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="8f85e-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="8f85e-110">Neem contact op met uw IT-beheerder als uw account geen beheerdersbevoegdheden van het bedrijf of facturering heeft.</span><span class="sxs-lookup"><span data-stu-id="8f85e-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
