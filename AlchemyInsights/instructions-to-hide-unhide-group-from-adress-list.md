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
# <a name="hide-office-365-group-from-address-list-gal"></a>Verberg Office 365 groep van adreslijst (GAL)

Als u een Office 365-groep wilt verbergen voor adreslijsten (GAL) van Exchange-clients (zoals Outlook of OWA), gebruikt u de volgende opdracht in EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Als u wilt verbergen dat de Office 365-groep zichtbaar is voor Exchange-clients, gebruikt u de volgende opdracht in EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

