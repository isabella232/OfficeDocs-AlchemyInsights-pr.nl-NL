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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910361"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Problemen met het delen SharePoint inhoud met externe gebruikers oplossen

Zorg ervoor dat extern delen is ingeschakeld voor uw organisatie:
  
1. Ga naar de [pagina &amp; Services-invoegvoegingen in de Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **Sites.**
    
2. Zorg ervoor dat de instelling is ingeschakeld op 'Aan'. Als 'Alleen bestaande externe gebruikers' is geselecteerd, moet u ervoor zorgen dat de externe gebruiker wordt weergegeven in de Microsoft 365-beheercentrum.
    
Zorg ervoor dat extern delen is ingeschakeld voor de site. Voor een klassieke siteverzameling:
  
1. Klik in het SharePoint in het linkerdeelvenster op **sites.**
    
2. Selecteer de site of sites en klik op het lint op **Delen.**
    
Voor een teamsite die deel uitmaken van een Microsoft 365 of een communicatiesite:
  
- Deze nieuwe sitetypen hebben dezelfde instelling voor delen als de instelling voor het hele bedrijf, tenzij u met de instelling voor de hele organisatie bestanden kunt delen met koppelingen waarvoor u zich niet hoeft aan te melden. In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden. Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-beheercentrum of PowerShell. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> De instelling voor extern delen voor een site kan beperkender zijn dan de instelling voor de hele organisatie, maar niet meer dan de instelling voor de hele organisatie. 
  

