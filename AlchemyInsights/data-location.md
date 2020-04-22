---
title: Gegevenslocatie
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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655277"
---
# <a name="data-location"></a>Gegevenslocatie

U de locatie van uw tenant bekijken in het beheercentrum of door verbinding te maken met Exchange Online via PowerShell.


**Beheercentrum:**
1. Log in bij het [beheercentrum](https://admin.microsoft.com/Adminportal/Home).
2. Selecteer Het profiel **van instellingenorganisatie** > **Organization profile**.
3. Selecteer **onder Gegevenslocatie**de optie **Details weergeven**.


**Powershell:**
1. Maak verbinding met Exchange Online met Windows PowerShell.
2. Voer de cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) uit om een lijst met de eigenschappen van uw tenant weer te geven. 
3. Kijk naar de OrganizationId eigendom.

Wanneer u de gegevenslocatie voor EXO en SPO hebt, u de gegevenslocatie bepalen voor andere services die u gebruiken vanaf [de plaats waar uw gegevens zich bevinden.](https://products.office.com/where-is-your-data-located)