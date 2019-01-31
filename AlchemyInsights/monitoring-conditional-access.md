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
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656562"
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
    
Meer informatie: [hoe apparaten Monitor voorwaardelijke toegang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

