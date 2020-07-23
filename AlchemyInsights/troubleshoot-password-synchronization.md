---
title: Problemen met wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387872"
---
# <a name="troubleshoot-password-synchronization"></a>Problemen met wachtwoordsynchronisatie oplossen

Als u problemen met wachtwoordsynchronisatie wilt oplossen, gebruikt u deze taak voor het oplossen van problemen met AAD Connect om te bepalen waarom wachtwoorden niet worden gesynchroniseerd. Ga om te beginnen naar [Directe synchronisatie beheren.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Open een nieuwe Windows PowerShell-sessie op uw Azure AD Connect-server en selecteer de optie **Uitvoeren als administrator.**

2. Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.

3. Start de wizard Azure AD Connect.

4. Ga naar de pagina Extra taken > **Volgende problemen oplossen**  >  **Next**.

5. Selecteer **Starten** om het menu Probleemoplossing van PowerShell te openen.

6. Selecteer **Wachtwoordsynchronisatie oplossen**.

    Het probleem is meestal dat een wachtwoord niet wordt gesynchroniseerd voor een specifiek gebruikersaccount.

    **Notities** Wachtwoordsynchronisatie mislukt als de laatste succesvolle wachtwoordsynchronisatie enige tijd geleden was.

Zie Problemen [met wachtwoordhashsynchronisatie oplossen met Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)voor meer hulp bij het oplossen van wachtwoordsynchronisatie.