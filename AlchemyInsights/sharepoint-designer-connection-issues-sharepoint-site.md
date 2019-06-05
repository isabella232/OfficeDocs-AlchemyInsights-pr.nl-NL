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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716887"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemen met SharePoint Designer 

<p>Als u SharePoint Designer ondervindt problemen met de verbinding met de SharePoint-sites, probeer dan de volgende gemeenschappelijke oplossingen.</p> <p><strong>Stap 1:</strong> <strong>Controleren of SharePoint Designer wordt bijgewerkt&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">Servicepack 1 (SP1) voor SharePoint Designer</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Update voor SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Stap 2:</strong> <strong>Wis de bestanden in de lokale cache</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Sluit de SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Ga naar de volgende mappen te verwijderen van bestanden in de cache op de lokale computer.&nbsp;</li> <li style="font-weight: 400;">Klik op <strong>Start -&gt; uitvoeren</strong> en verwijder alle bestanden gevonden in elk van de onderstaande locaties.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">SharePoint Designer 2013 openen en geef de account opnieuw om te zien als het werkt.</li> </ol> <p><strong>Stap 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Moderne voor Office 2013 op apparaten met Windows-verificatie inschakelen</strong></a>&nbsp;</p> <p><strong>Stap 4:</strong> <strong>Beheerders moeten aangepast Script waarmee de verbinding met SharePoint Designer toestaan</strong>.</p> <p>Zie voor gedetailleerde stappen, voorbeelden en overwegingen <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">toestaan of voorkomen van aangepast script</a>.&nbsp;</p>


