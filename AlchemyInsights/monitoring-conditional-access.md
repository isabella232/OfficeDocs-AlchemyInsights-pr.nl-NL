---
title: Toezicht op voorwaardelijke toegang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464833"
---
# <a name="monitoring-conditional-access"></a>Toezicht op voorwaardelijke toegang

Gericht met voorwaardelijke toegang ontvangen gebruikers een melding per e-mail als zij niet voldoen aan de toegangsvereisten van uw organisatie. Als u wilt oplossen, raden we aan een of meer van de volgende oplossingen:
  
- Als het apparaat wordt verondersteld te worden ingeschreven, adviseren de gebruiker naar de bedrijfsportal app gaan en controleren of deze wordt weergegeven in de bedrijfsportal. Als dat niet het geval is, moet de gebruiker het apparaat inschrijven.
    
- Ga in de Azure portal naar **Intune \> apparaat naleving**. Klik op **apparaat conformiteit**onder **Monitor** . Bekijk uw conformiteitsrapport apparaat om te controleren dat het apparaat van de gebruiker is gemarkeerd als compatibel. 
    
- Ga in de Azure portal naar **Intune \> apparaat naleving**. Klik onder **beheren**, klikt u op het **beleid**. Controleren of een profiel is toegewezen aan het apparaat van de gebruiker in de lijst van het beleid voldaan. Als er geen profiel is toegewezen, vervolgens Intune worden niet kunnen bevestigen de bestendigheid van het apparaat. 
    
- Bewerken van voorwaardelijke toegang van de gebruiker is toegewezen.
    
1. Ga in de Azure portal naar **Intune \> voorwaardelijke toegang \> beleid**
    
2. Selecteer een beleid in de lijst
    
3. Klik op **gebruikers en groepen**
    
4. Als een bepaald beleid op iemand anders, moet u deze aan **de lijst** toevoegen. Om ervoor te zorgen dat een persoon wordt weggelaten uit het beleid, toevoegen aan de lijst **uitgesloten** . 
    
Meer informatie: [hoe apparaten Monitor voorwaardelijke toegang](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

