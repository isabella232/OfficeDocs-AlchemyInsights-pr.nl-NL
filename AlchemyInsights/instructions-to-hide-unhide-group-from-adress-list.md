---
title: Instructies voor het verbergen/weergeven van een groep in de adreslijst
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926240"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>De Microsoft 365 groep verbergen in adreslijst (GAL)

Als u een Microsoft 365 groep wilt verbergen voor adreslijsten (GAL) van Exchange-clients (zoals Outlook of OWA), gebruikt u de volgende opdracht in EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Als u wilt verbergen Microsoft 365 groep zichtbaar is voor Exchange clients, gebruikt u de volgende opdracht in EXO-shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

