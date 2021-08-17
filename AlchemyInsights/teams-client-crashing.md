---
title: Teams client vast loopt
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890333"
---
# <a name="teams-client-crashing"></a>Teams client vast loopt

Als uw Teams-client crasht, probeer dan het volgende:

- Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Zorg ervoor dat alle [Microsoft 365 URL's en adresbereiken](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.

- Meld u aan met uw tenantbeheerderaccount en controleer uw [Service health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.

- De Teams verwijderen en opnieuw installeren
    - Blader naar de map %appdata%\Microsoft\Teams\ op uw computer en verwijder alle bestanden in die map.
    - [Download en installeer de Teams-app](https://www.microsoft.com/microsoft-teams/download-app)en installeer Teams indien mogelijk als beheerder (klik met de rechtermuisknop op het Teams-installatieprogramma en selecteer Uitvoeren als **beheerder** indien beschikbaar).

Als uw Teams nog steeds vast loopt, probeert u het probleem te reproduceren. Als u het volgende kunt doen:

1. Gebruik de stappenrecorder om uw stappen vast te leggen.
    - Sluit ALLE overbodige of vertrouwelijke toepassingen.
    - Start de stappenrecorder en reproduceer het probleem terwijl u bent aangemeld met het betreffende gebruikersaccount.
    - [Verzamel de teamslogboeken die de vastgelegde reprostappen vastleggen.](https://docs.microsoft.com/microsoftteams/log-files) **Opmerking:** Zorg ervoor dat u het aanmeldingsadres van de beïnvloede gebruiker vast legt.
    - Verzamel de dump- en/of foutemmergegevens (Windows). Start Windows Powershell op de computer waar de crash plaatsvindt en voer de volgende opdrachten uit (druk na elke opdracht op Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Nadat het tekstbestand is gegenereerd en op het scherm wordt weergegeven, kunt u het bestand opslaan en toevoegen aan de serviceaanvraag. 
