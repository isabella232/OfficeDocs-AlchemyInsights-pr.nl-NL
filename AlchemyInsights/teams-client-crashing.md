---
title: Teams-cliënt crasht?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354047"
---
# <a name="teams-client-crashing"></a>Teams-cliënt crasht?

Als uw Teams-client crasht, probeer dan het volgende:

- Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Zorg ervoor dat alle [Microsoft 365-URL's en adresbereiken](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.

- Meld u aan met uw tenantadmin-account en controleer uw [dashboard servicestatus](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.

- De Teams-toepassing verwijderen en opnieuw installeren (koppeling)
    - Blader naar de map %appdata%\Microsoft\teams\ op uw computer en verwijder alle bestanden in die map.
    - [Download en installeer de Teams-app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)en installeer teams indien mogelijk als beheerder (klik met de rechtermuisknop op het installatieprogramma Teams en selecteer 'Uitvoeren als beheerder' indien beschikbaar).

Als uw Teams-client nog steeds crasht, u het probleem reproduceren? Zo ja:

1. Gebruik de Steps Recorder om uw stappen vast te leggen.
    - Sluit ALLE onnodige of vertrouwelijke toepassingen.
    - Start de Steps Recorder en reproduceren het probleem terwijl ingelogd met de getroffen gebruikersaccount.
    - [Verzamel de teams logs die de opgenomen repro stappen vast te leggen](https://docs.microsoft.com/microsoftteams/log-files). **Opmerking:** zorg ervoor dat u het aanmeldingsadres van de getroffen gebruiker vastlegt.
    - Verzamel de dump- en/of foutbucket-informatie (Windows). Start Windows Powershell op de machine waar de crash plaatsvindt en voer de volgende opdrachten uit:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Voeg het bestand toe aan uw ondersteuningsaanvraag.
