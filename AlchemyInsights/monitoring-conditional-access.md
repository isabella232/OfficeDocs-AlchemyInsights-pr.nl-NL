---
title: Voorwaardelijke toegang controleren
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702898"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Voorwaardelijke toegang voor Exchange controleren

Gebruikers met voorwaardelijke toegang ontvangen een e-mail melding als ze niet voldoen aan de toegangsvereisten van uw organisatie. We raden een of meer van de volgende oplossingen aan om dit op te lossen:
  
- Als u ervan wordt uitgegaan dat het apparaat is ingeschreven, adviseert u de gebruiker om naar de bedrijfsportal-app te gaan en controleert u of deze wordt weergegeven in de bedrijfsportal. Als dit niet het geval is, moet de gebruiker het apparaat registreren.
    
- Ga in de Azure-Portal naar **naleving van intune- \> apparaten**. Klik **Monitor** onder monitor **op apparaatcompatibiliteit**. Bekijk het nalevings rapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel. 
    
- Ga in de Azure-Portal naar **naleving van intune- \> apparaten**. Klik onder **beheren**op **beleidsregels**. Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruikers. Als u geen profiel hebt toegewezen, kan intune de nalevingsstatus van het apparaat niet bevestigen. 
    
- De voorwaardelijke toegang-opdracht van de gebruiker bewerken.
    
1. Ga in de Azure-Portal naar **intune- \> \> beleid voor voorwaardelijke toegang**
    
2. Selecteer een beleid in de lijst.
    
3. Klik op **gebruikers en groepen**
    
4. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe **aan de lijst toevoegen.** Voeg ze toe aan de lijst **uitsluiten** om ervoor te zorgen dat iemand van het beleid weglaat. 
    
Meer informatie: [voorwaardelijke toegangs apparaten volgen](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

