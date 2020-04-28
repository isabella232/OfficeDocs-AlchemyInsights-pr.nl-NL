---
title: Delen met externe gebruikers werkt niet
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912997"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Problemen oplossen bij het delen van SharePoint-inhoud met externe gebruikers

Controleer of extern delen is ingeschakeld voor uw organisatie:
  
1. Ga naar de [pagina Invoegtoepassing &amp; Services in het Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **Sites**.
    
2. Controleer of de instelling is ingeschakeld in 'Aan'. Als 'Alleen bestaande externe gebruikers' is geselecteerd, controleert u of de externe gebruiker wordt vermeld in het Microsoft 365-beheercentrum.
    
Zorg ervoor dat extern delen is ingeschakeld voor de site. Voor een klassieke site collectie:
  
1. Klik in het nieuwe SharePoint-beheercentrum in het linkerdeelvenster op **sites**.
    
2. Selecteer de site of sites en klik op het lint op **Delen**.
    
Voor een teamsite die deel uitmaakt van een Microsoft 365-groep of een communicatiesite:
  
- Deze nieuwe sitetypen hebben dezelfde instelling voor delen als de instelling voor uw hele organisatie, tenzij de instelling voor de hele organisatie het delen van bestanden toestaat met koppelingen waarvoor geen aanmelding vereist is. In dit geval staan de sites het delen toe met nieuwe en bestaande externe gebruikers die zich aanmelden. Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-beheercentrum of PowerShell. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> De instelling voor extern delen voor elke site kan restrictiever zijn dan uw organisatiebrede instelling, maar niet toleranter dan de organisatiebrede instelling. 
  

