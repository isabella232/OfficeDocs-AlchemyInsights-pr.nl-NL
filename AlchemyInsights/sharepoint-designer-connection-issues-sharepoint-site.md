---
title: Problemen met SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508418"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemen met SharePoint Designer 

Als u SharePoint Designer ondervindt problemen met de verbinding met de SharePoint-sites, probeert u de volgende algemene oplossingen.

Stap 1: Controleren of SharePoint Designer 2013 is bijgewerkt met [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) en [2 augustus 2016 bijwerken voor SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Stap 2: Wis de bestanden in de lokale cache:

1. Sluit de SharePoint Designer 2013.

2. Verwijder alle bestanden in de volgende mappen op de lokale computer.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013 openen en geef de account opnieuw om te zien als het werkt.

Stap 3: [moderne-verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Stap 4: Beheerders moet **Toestaan aangepast Script** in de Admin Center van SharePoint instellingen voor de verbinding van SharePoint Designer toestaan. Zie [toestaan of voorkomen van aangepast script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) voor meer informatie.


