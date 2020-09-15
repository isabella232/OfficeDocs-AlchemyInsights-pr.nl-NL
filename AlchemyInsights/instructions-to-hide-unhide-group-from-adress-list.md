---
title: Instructies voor het weergeven of zichtbaar maken van de groep van de adreslijst
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663004"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="cc249-102">Groep Microsoft 365 verbergen in de adreslijst (GAL)</span><span class="sxs-lookup"><span data-stu-id="cc249-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="cc249-103">Als u een Microsoft 365-groep wilt verbergen voor de adreslijsten (GAL) van Exchange-clients (zoals Outlook of OWA), gebruikt u de volgende opdracht in EXO shell:</span><span class="sxs-lookup"><span data-stu-id="cc249-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="cc249-104">Als u wilt dat de Microsoft 365-groep wordt weergegeven voor Exchange-clients, gebruikt u de volgende opdracht in EXO shell:</span><span class="sxs-lookup"><span data-stu-id="cc249-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

