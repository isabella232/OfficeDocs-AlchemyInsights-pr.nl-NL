---
title: Delen met externe gebruikers werkt niet
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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502226"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Problemen met het delen van SharePoint-inhoud met externe gebruikers oplossen

Zorg ervoor dat extern delen is ingeschakeld voor uw organisatie:
  
1. Ga naar de [pagina &amp; Services-invoegtoepassingen in het Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **sites**.
    
2. Zorg ervoor dat de instelling is ingeschakeld op ' aan '. Als ' alleen bestaande externe gebruikers ' is geselecteerd, controleert u of de externe gebruiker wordt vermeld in het Microsoft 365 Admin Center.
    
Zorg ervoor dat extern delen is ingeschakeld voor de site. Voor een klassieke siteverzameling:
  
1. In het nieuwe SharePoint-Beheercentrum, in het linkerdeelvenster, klikt u op **sites**.
    
2. Selecteer de site of sites en klik op het lint op **delen**.
    
Voor een team site die behoort tot een Office 365-groep of een communicatiesite:
  
- Deze nieuwe site typen hebben dezelfde instelling voordelen als de instelling voor de hele organisatie, tenzij de organisatiebrede instelling het delen van bestanden toestaat met behulp van koppelingen die niet hoeven te worden aangemeld. In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden. Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-Beheercentrum of PowerShell. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> De instelling voor extern delen voor elke site kan restrictiever zijn dan de instelling van de hele organisatie, maar niet meer toelaatbaar dan de organisatiebrede instelling. 
  

