---
title: Problemen met wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732505"
---
# <a name="troubleshoot-password-synchronization"></a>Problemen met wachtwoordsynchronisatie oplossen

Problemen oplossen waarbij geen wachtwoorden worden gesynchroniseerd met Azure AD Connect-versie 1.1.614.0 of hoger:
  
1. Open een nieuwe Windows PowerShell-sessie op uw Azure AD Connect-server met de optie **Uitvoeren als administrator.**

2. **Uitvoeren Set-ExecutionPolicy RemoteSigned** of **Set-ExecutionPolicy onbeperkt**uitvoeren .

3. Start de wizard Azure AD Connect.

4. Navigeer naar de pagina **Extra taken,** selecteer **Problemen oplossen**en klik op **Volgende**.

5. Klik op de pagina Probleemoplossing op Starten om het menu probleemoplossing in PowerShell **te starten.**

6. Selecteer in het hoofdmenu **Problemen met wachtwoordsynchronisatie oplossen**.

7. Selecteer **Wachtwoordsynchronisatie werkt helemaal niet in**het submenu.

**De resultaten van de probleemoplossingstaak begrijpen**
  
De taak voor het oplossen van problemen voert de volgende controles uit:
  
- Valideert dat de functie voor wachtwoordsynchronisatie is ingeschakeld voor uw Azure AD-tenant.

- Valideert dat de Azure AD Connect-server zich niet in de faseringsmodus bevindt.

- Voor elke bestaande on-premises Active Directory-connector (die overeenkomt met een bestaand Active Directory-forest):

- 
  - Hiermee wordt gevalideerd dat de functie wachtwoordsynchronisatie is ingeschakeld.

  - Hiermee wordt gezocht naar heartbeatgebeurtenissen voor wachtwoordsynchronisatie in de logboeken van Windows Application Event.

  - Voor elk Active Directory-domein onder de on-premises Active Directory-connector:

  - Valideert dat het domein bereikbaar is vanaf de Azure AD Connect-server.

  - Hiermee wordt gevalideerd dat de AD DS-accounts (Active Directory Domain Services) die worden gebruikt door de on-premises Active Directory-connector de juiste gebruikersnaam, wachtwoord en machtigingen hebben die nodig zijn voor wachtwoordsynchronisatie.

Zie [Wachtwoordsynchronisatie oplossen met Azure AD Connect-synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)voor meer hulp bij het oplossen van problemen met wachtwoordsynchronisatie.
  