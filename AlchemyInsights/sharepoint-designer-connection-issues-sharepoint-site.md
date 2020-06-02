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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511539"
---
# <a name="sharepoint-designer-connection-issues"></a>Verbindingsproblemen met SharePoint Designer 

Als SharePoint Designer verbindingsproblemen ondervindt met SharePoint-sites, probeert u de volgende algemene oplossingen.

Stap 1: Controleer of SharePoint Designer 2013 is bijgewerkt met [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) en de [update van 2 augustus 2016 voor SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Stap 2: De lokale cachebestanden wissen:

1. Sluit SharePoint Designer 2013.

2. Verwijder op de lokale computer alle bestanden die in elk van de volgende mappen worden gevonden.

    - %APPDATA%\Microsoft\Webserverextensies\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Open SharePoint Designer 2013 en voer het account opnieuw in om te zien of het werkt.

Stap 3: [Moderne verificatie voor Office 2013 inschakelen op Windows-apparaten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Stap 4: Beheerders moeten **aangepast script toestaan** in de instellingen van het SharePoint-beheercentrum om de SharePoint Designer-verbinding toe te staan. Zie [Aangepast script toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.


