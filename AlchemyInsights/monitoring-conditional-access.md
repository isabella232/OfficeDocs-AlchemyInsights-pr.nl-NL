---
title: Controle voorwaardelijke toegang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713713"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Controle op voorwaardelijke toegang voor Exchange

Gebruikers die zijn getarget met voorwaardelijke toegang, ontvangen een e-mail met een melding als ze niet voldoen aan de toegangsvereisten van uw organisatie. Om het probleem op te lossen, raden we een of meer van de volgende oplossingen aan:
  
- Als het apparaat wordt verondersteld te zijn ingeschreven, adviseert u de gebruiker om naar de App Van bedrijfsportal te gaan en te verifiëren of het in de bedrijfsportal wordt weergegeven. Als dit niet het zo is, moet de gebruiker het apparaat inschrijven.
    
- Ga in de Azure-portal naar **Intune \> Device compliance**. Klik **onder Controleren** op Naleving van het **apparaat**. Bekijk het nalevingsrapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel. 
    
- Ga in de Azure-portal naar **Intune \> Device compliance**. Klik **onder Beheren**op **Beleid**. Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruiker. Als er geen profiel is toegewezen, kan Intune de nalevingsstatus van het apparaat niet bevestigen. 
    
- De voorwaardelijke toegangstoewijzing van de gebruiker bewerken.
    
1. Ga in de Azure-portal naar **Intune-beleid \> \> voor voorwaardelijke toegang**
    
2. Een beleid selecteren in de lijst
    
3. Klik **op Gebruikers en groepen**
    
4. Als u een bepaald beleid op iemand wilt targeten, voegt u deze toe aan de lijst **Opnemen.** Als u ervoor wilt zorgen dat een persoon uit het beleid wordt weggelaten, voegt u deze toe aan de lijst **Uitsluiten.** 
    
Lees meer: [Apparaten voor voorwaardelijke toegang controleren](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

