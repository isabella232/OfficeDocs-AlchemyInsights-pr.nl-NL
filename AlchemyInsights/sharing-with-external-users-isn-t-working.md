---
title: Delen met externe gebruikers werkt niet.
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369493"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-inhoud delen met externe gebruikers problemen oplossen

Zorg ervoor dat externe delen is ingeschakeld voor uw organisatie:
  
1. Ga naar de [Services &amp; pagina-ins in het Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), en op **websites**.
    
2. Controleer of dat de instelling is ingeschakeld op 'Aan'. Als 'Alleen bestaande externe gebruikers' is ingeschakeld, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365 admin center.
    
Zorg ervoor dat extern delen die zijn ingeschakeld voor de site. Voor een klassieke siteverzameling:
  
1. Klik in het nieuwe SharePoint admin center, in het linkerdeelvenster op **websites**.
    
2. Selecteer de site of sites en op het lint, klik op **delen**.
    
Voor een teamsite die behoort tot een groep van Office 365, of een communicatiesite:
  
- Deze nieuwe site typen hebben de dezelfde delen als u als instelling voor de hele organisatie, tenzij u de instelling van de hele organisatie ondersteunt het delen van bestanden via de koppelingen die niet vereisen-in. In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden. U wijzigt de instelling voor specifieke sites, moet u de nieuwe SharePoint admin center of PowerShell gebruiken. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> De externe delen instellen voor elke site is meer beperkend zijn dan de instelling voor de hele organisatie, maar niet meer dan de instelling voor de hele organisatie strikte. 
  

