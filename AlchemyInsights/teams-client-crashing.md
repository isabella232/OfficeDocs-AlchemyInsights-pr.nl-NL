---
title: Teams client loopt vast
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187716"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a15f8-102">Teams client loopt vast</span><span class="sxs-lookup"><span data-stu-id="a15f8-102">Teams client crashing</span></span>

<span data-ttu-id="a15f8-103">Als uw Teams-client crasht, probeer dan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a15f8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a15f8-104">Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a15f8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a15f8-105">Zorg ervoor dat alle [Microsoft 365 URL's en adresbereiken](/microsoftteams/connectivity-issues) toegankelijk zijn.</span><span class="sxs-lookup"><span data-stu-id="a15f8-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a15f8-106">Meld u aan met uw tenantbeheerderaccount en controleer uw [Service Health Dashboard](/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.</span><span class="sxs-lookup"><span data-stu-id="a15f8-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="a15f8-107">De toepassing verwijderen en opnieuw Teams installeren</span><span class="sxs-lookup"><span data-stu-id="a15f8-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="a15f8-108">Blader naar de map %appdata%\Microsoft\Teams\ op uw computer en verwijder alle bestanden in die adreslijst.</span><span class="sxs-lookup"><span data-stu-id="a15f8-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="a15f8-109">[Download en installeer de Teams-app](https://www.microsoft.com/microsoft-teams/download-app)en installeer Teams indien mogelijk als beheerder (klik met de rechtermuisknop op het Teams-installatieprogramma en selecteer Uitvoeren als **beheerder** indien beschikbaar).</span><span class="sxs-lookup"><span data-stu-id="a15f8-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="a15f8-110">Als uw Teams nog steeds vast loopt, probeert u het probleem te reproduceren.</span><span class="sxs-lookup"><span data-stu-id="a15f8-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="a15f8-111">Als u het volgende kunt doen:</span><span class="sxs-lookup"><span data-stu-id="a15f8-111">If you can:</span></span>

1. <span data-ttu-id="a15f8-112">Gebruik de stappenrecorder om uw stappen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="a15f8-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="a15f8-113">Sluit ALLE overbodige of vertrouwelijke toepassingen.</span><span class="sxs-lookup"><span data-stu-id="a15f8-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="a15f8-114">Start de stappenrecorder en reproduceer het probleem terwijl u bent aangemeld met het betreffende gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="a15f8-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="a15f8-115">[Verzamel de teamslogboeken die de vastgelegde reprostappen vastleggen.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="a15f8-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="a15f8-116">**Opmerking:** Zorg ervoor dat u het aanmeldingsadres van de beïnvloede gebruiker vast legt.</span><span class="sxs-lookup"><span data-stu-id="a15f8-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="a15f8-117">Verzamel de dump- en/of foutemmergegevens (Windows).</span><span class="sxs-lookup"><span data-stu-id="a15f8-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="a15f8-118">Start Windows Powershell op de computer waar de crash plaatsvindt en voer de volgende opdrachten uit (druk na elke opdracht op Enter):</span><span class="sxs-lookup"><span data-stu-id="a15f8-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="a15f8-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="a15f8-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="a15f8-120">Nadat het tekstbestand is gegenereerd en op het scherm wordt weergegeven, kunt u het bestand opslaan en toevoegen aan de serviceaanvraag.</span><span class="sxs-lookup"><span data-stu-id="a15f8-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
