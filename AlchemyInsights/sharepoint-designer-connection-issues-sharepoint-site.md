---
title: Verbindingsproblemen met SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727166"
---
# <a name="sharepoint-designer-connection-issues"></a>Verbindingsproblemen met SharePoint Designer 

Als SharePoint Designer verbindingsproblemen met SharePoint-sites ondervindt, kunt u de volgende veelgebruikte oplossingen proberen.

Stap 1: Controleer of SharePoint Designer 2013 is bijgewerkt met [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) en de [Update van 2 augustus 2016 voor sharepoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Stap 2: de lokale cachebestanden wissen:

1. Sluit SharePoint Designer 2013.

2. Op de lokale computer verwijdert u alle bestanden die zijn gevonden in de volgende mappen.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Open SharePoint Designer 2013 en voer het account opnieuw in om te zien of het werkt.

Stap 3: [moderne verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Stap 4: beheerders dienen **aangepaste scripts toe te staan** in de SharePoint-Beheercentrum-instellingen om de verbinding met SharePoint Designer toe te staan. Zie [aangepaste scripts toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.


