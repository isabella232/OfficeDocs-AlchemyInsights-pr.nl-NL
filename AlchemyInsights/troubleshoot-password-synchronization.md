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
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924691"
---
# <a name="troubleshoot-password-synchronization"></a>Problemen met Wachtwoordsynchronisatie oplossen

Problemen waar geen wachtwoorden gesynchroniseerd met Azure AD verbinden versie 1.1.614.0 of hoger worden:
  
1. Open een nieuwe Windows PowerShell-sessie op de server Azure AD verbinding maken met de optie **als Administrator uitvoeren** . 
    
2. **Set uitvoeringsbeleid RemoteSigned** of **onbeperkte Set uitvoeringsbeleid**uitvoeren. 
    
3. Start de wizard Azure AD verbinden.
    
4. Ga naar de ** extra taken ** Selecteer pagina ** oplossen **, en klik op **volgende**. 
    
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
  

