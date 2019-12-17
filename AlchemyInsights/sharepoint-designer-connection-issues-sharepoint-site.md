---
title: Verbindingsproblemen met SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051708"
---
# <a name="sharepoint-designer-connection-issues"></a>Verbindingsproblemen met SharePoint Designer 

Als SharePoint Designer verbindingsproblemen ondervindt met SharePoint-sites, probeert u de volgende algemene oplossingen.

Stap 1: Controleer of SharePoint Designer 2013 is bijgewerkt met [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) en de [Update 2, 2016 voorsharepoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Stap 2: wis de lokale cachebestanden:

1. Sluit SharePoint Designer 2013.

2. Verwijder alle bestanden die in de volgende mappen zijn gevonden op de lokale computer.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Open SharePoint Designer 2013 en voer het account opnieuw in om te zien of het werkt.

Stap 3: [Schakel moderne verificatie voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Stap 4: beheerders moeten het **aangepaste script toestaan** in de instellingen van het SharePoint Admin Center om de SharePoint Designer-verbinding toe te staan. Zie [aangepast script toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.


