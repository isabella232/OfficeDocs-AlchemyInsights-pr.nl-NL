---
title: Verbinding maken met de MSCommerce-module
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702610"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="1c1ce-102">Voor MSCommerce is een account van een beheerder voor bedrijven of facturering vereist</span><span class="sxs-lookup"><span data-stu-id="1c1ce-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="1c1ce-103">Voor de MSCommerce-module is een account met beheerdersbevoegdheden voor de beheerder of de beheerder vereist.</span><span class="sxs-lookup"><span data-stu-id="1c1ce-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="1c1ce-104">Als de volgende fout wordt weergegeven, moet u opnieuw verbinding maken met een ander account.</span><span class="sxs-lookup"><span data-stu-id="1c1ce-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="1c1ce-105">*ErrorMessage-de externe server heeft een fout geretourneerd: (403) niet toegestaan. ErrorDetails-in C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 tekens: 5*</span><span class="sxs-lookup"><span data-stu-id="1c1ce-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="1c1ce-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $ _-CustomErrorMessage "kon niet worden retri...*</span><span class="sxs-lookup"><span data-stu-id="1c1ce-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="1c1ce-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="1c1ce-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="1c1ce-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Schrijffout]; WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="1c1ce-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="1c1ce-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. Command. WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="1c1ce-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="1c1ce-110">Neem contact op met uw IT-beheerder als u geen beheerdersrechten hebt voor uw account.</span><span class="sxs-lookup"><span data-stu-id="1c1ce-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
