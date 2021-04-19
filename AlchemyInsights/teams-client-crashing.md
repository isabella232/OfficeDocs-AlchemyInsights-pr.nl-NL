---
title: Teams-cliënt crasht?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826266"
---
# <a name="teams-client-crashing"></a>Teams-cliënt crasht?

Als uw Teams-client crasht, probeer dan het volgende:

- Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Zorg ervoor dat alle URL's en adresbereiken van [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.

- Meld u aan met uw tenantbeheerderaccount en controleer uw [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.

- De Teams-toepassing verwijderen en opnieuw installeren (koppeling)
    - Blader naar de map %appdata%\Microsoft\teams\ op uw computer en verwijder alle bestanden in die adreslijst.
    - [Download en installeer de Teams-app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)en installeer Teams indien mogelijk als beheerder (klik met de rechtermuisknop op het Installatieprogramma van Teams en selecteer 'Uitvoeren als beheerder' indien beschikbaar).

Als uw Teams-client nog steeds vast loopt, kunt u het probleem dan reproduceren? Zo ja:

1. Gebruik de stappenrecorder om uw stappen vast te leggen.
    - Sluit ALLE overbodige of vertrouwelijke toepassingen.
    - Start de stappenrecorder en reproduceer het probleem terwijl u bent aangemeld met het betreffende gebruikersaccount.
    - [Verzamel de teamslogboeken die de vastgelegde reprostappen vastleggen.](https://docs.microsoft.com/microsoftteams/log-files) **Opmerking:** Zorg ervoor dat u het aanmeldingsadres van de beïnvloede gebruiker vast legt.
    - Verzamel de dump- en/of foutemmergegevens (Windows). Start Windows Powershell op de computer waar de crash plaatsvindt en voer de volgende opdrachten uit:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Voeg het bestand toe aan uw ondersteuningscase.
