---
title: Delen met externe gebruikers werkt niet
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691570"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Problemen oplossen met het delen van SharePoint-inhoud met externe gebruikers

Zorg ervoor dat extern delen is ingeschakeld voor uw organisatie:
  
1. Ga naar de [ &amp; pagina invoegtoepassingen voor services in het microsoft 365-Beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **sites**.
    
2. Zorg dat de instelling is ingeschakeld op aan. Als ' alleen bestaande externe gebruikers ' is geselecteerd, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365-Beheercentrum.
    
Zorg ervoor dat extern delen is ingeschakeld voor de site. Voor een klassieke siteverzameling:
  
1. Klik in het nieuwe SharePoint-Beheercentrum in het linkerdeelvenster op **sites**.
    
2. Selecteer de site of sites en klik op het lint op **delen**.
    
Voor een team site die hoort bij een Microsoft 365-groep, of een communicatiesite:
  
- Deze nieuwe site typen hebben dezelfde instelling voordelen als de instelling voor de gehele organisatie, tenzij de instelling voor hele organisatie het delen van bestanden toestaat met behulp van koppelingen waarvoor aanmelding niet is vereist. In dit geval kunnen de sites delen delen met nieuwe en bestaande externe gebruikers die zich aanmelden. Gebruik het nieuwe SharePoint-Beheercentrum of PowerShell om de instelling voor specifieke sites te wijzigen. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> De instelling voor extern delen voor een site kan meer beperkingen zijn dan de instelling voor de gehele organisatie, maar niet meer beperkt dan de instelling voor de gehele organisatie. 
  

