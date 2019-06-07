---
title: Machtigingsniveaus voor SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760688"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemen met SharePoint Designer 

Als u SharePoint Designer ondervindt problemen met de verbinding met de SharePoint-sites, probeer dan de volgende gemeenschappelijke oplossingen.

Stap 1: Controleer of SharePoint Designer wordt bijgewerkt.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [Servicepack 1 (SP1) voor SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Update voor SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Stap 2: Wis de bestanden in de lokale cache

- Sluit de SharePoint Designer 2013.

- Ga naar de volgende mappen te verwijderen van bestanden in de cache op de lokale computer.

- Klik op Start, uitvoeren en verwijderen, alle bestanden in elk van gevonden de onderstaande locaties.

%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

SharePoint Designer 2013 openen en geef de account opnieuw om te zien als het werkt.

Stap 3: [moderne voor Office 2013 op apparaten met Windows-verificatie inschakelen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Stap 4: Beheerders moet aangepast Script dat de verbinding van SharePoint Designer toestaan.

Zie voor gedetailleerde stappen, voorbeelden en overwegingen [toestaan of voorkomen van aangepast script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


