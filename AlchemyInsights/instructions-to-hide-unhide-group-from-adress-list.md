---
title: Instructies voor het verbergen/zichtbaar maken van groep van adreslijst
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768912"
---
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="b7479-102">Verberg Office 365 groep van adreslijst (GAL)</span><span class="sxs-lookup"><span data-stu-id="b7479-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="b7479-103">Als u een Office 365-groep wilt verbergen voor adreslijsten (GAL) van Exchange-clients (zoals Outlook of OWA), gebruikt u de volgende opdracht in EXO shell:</span><span class="sxs-lookup"><span data-stu-id="b7479-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="b7479-104">Als u wilt verbergen dat de Office 365-groep zichtbaar is voor Exchange-clients, gebruikt u de volgende opdracht in EXO shell:</span><span class="sxs-lookup"><span data-stu-id="b7479-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

