---
title: Problemen met Wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533802"
---
# <a name="troubleshoot-password-synchronization"></a>Problemen met Wachtwoordsynchronisatie oplossen

Problemen waar geen wachtwoorden gesynchroniseerd met Azure AD verbinden versie 1.1.614.0 of hoger worden:
  
1. Open een nieuwe Windows PowerShell-sessie op de server Azure AD verbinding maken met de optie **als Administrator uitvoeren** .

2. **Set uitvoeringsbeleid RemoteSigned** of **onbeperkte Set uitvoeringsbeleid**uitvoeren.

3. Start de wizard Azure AD verbinden.

4. Ga naar de pagina **Meer taken** , **problemen met**selecteren en op **volgende**.

5. Klik op de pagina probleemoplossing menu **starten om te beginnen met het oplossen van problemen** in PowerShell.

6. Selecteer in het hoofdmenu **Password Synchronization oplossen**.

7. Selecteer **Wachtwoordsynchronisatie werkt niet op alle**in de submenu.

**Inzicht in de resultaten van de taak voor het oplossen van problemen**
  
De taak voor het oplossen van problemen worden de volgende controles uitgevoerd:
  
- Dat de functie wachtwoord synchronisatie is ingeschakeld voor uw huurder Azure AD worden gevalideerd.

- Valideert de Azure AD Connect-server is niet in een staging-modus.

- Voor elke bestaande op ruimten Active Directory-connector (die overeenkomt met een bestaande Active Directory-forest):

- 
  - Controleert of de functie wachtwoord synchronisatie is ingeschakeld.

  - Zoekt u wachtwoord synchronisatiegebeurtenissen heartbeat in de gebeurtenislogboeken van Windows-toepassing.

  - Voor elk Active Directory-domein in Active Directory-connector op de lokalen:

  - Wordt gecontroleerd of het domein bereikbaar is vanaf de server verbinden met Azure AD.

  - Wordt gecontroleerd of de Active Directory Domain Services (AD DS) rekeningen die worden gebruikt door Active Directory-connector op de ruimten heeft de juiste gebruikersnaam, wachtwoord en machtigingen vereist voor de synchronisatie van wachtwoorden.

Zie voor meer informatie het wachtwoord synchronisatie oplossen [problemen met Wachtwoordsynchronisatie met Azure AD verbinden synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  