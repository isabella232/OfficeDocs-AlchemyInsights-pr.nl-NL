---
title: Locatie van gegevens
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207256"
---
# <a name="data-location"></a>Locatie van gegevens

U de locatie van uw Office 365-Tenant weergeven in het Admin Center of door verbinding te maken met Exchange Online via PowerShell.


**Admin Center:**
1. Meld u aan bij het [Admin Center](https://admin.microsoft.com/Adminportal/Home).
2. Selecteer **instellingen** > **organisatie profiel**.
3. Selecteer onder **gegevenslocatie**de optie **Details weergeven**.


**Powershell:**
1. Verbinding maken met Exchange Online met behulp van Windows PowerShell.
2. Voer de cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) om een lijst met de eigenschappen van uw Tenant weer te geven. 
3. Bekijk de eigenschap OrganizationId.

Wanneer u de gegevenslocatie voor EXO en SPO hebt, u de gegevenslocatie bepalen voor andere services die u gebruiken vanaf [waar uw gegevens zich bevinden](https://products.office.com/where-is-your-data-located).