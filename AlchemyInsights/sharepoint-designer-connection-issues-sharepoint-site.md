---
title: SharePoint Problemen met designerverbinding
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942020"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemen met designerverbinding 

Als SharePoint designer verbindingsproblemen ondervindt met SharePoint sites, kunt u de volgende algemene oplossingen proberen.

Stap [1:](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) Controleer of SharePoint Designer 2013 is bijgewerkt met SharePoint Designer Service Pack 1 en de update van 2 augustus [2016 voor SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Stap 2: De lokale cachebestanden wissen:

1. Sluit SharePoint Designer 2013.

2. Verwijder op de lokale computer alle bestanden die in elk van de volgende mappen zijn gevonden.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Open SharePoint Designer 2013 en voer het account opnieuw in om te zien of het werkt.

Stap 3: Moderne verificatie [inschakelen voor Office 2013 op Windows apparaten.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Stap 4: Beheerders moeten aangepast **script** toestaan in de instellingen SharePoint beheercentrum om de SharePoint Designer-verbinding toe te staan. Zie [Aangepaste scripts toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.


