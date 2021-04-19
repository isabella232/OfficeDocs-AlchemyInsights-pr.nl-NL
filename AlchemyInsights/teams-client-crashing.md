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
# <a name="teams-client-crashing"></a><span data-ttu-id="b3634-102">Teams-cliënt crasht?</span><span class="sxs-lookup"><span data-stu-id="b3634-102">Teams client crashing?</span></span>

<span data-ttu-id="b3634-103">Als uw Teams-client crasht, probeer dan het volgende:</span><span class="sxs-lookup"><span data-stu-id="b3634-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="b3634-104">Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="b3634-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="b3634-105">Zorg ervoor dat alle URL's en adresbereiken van [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.</span><span class="sxs-lookup"><span data-stu-id="b3634-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="b3634-106">Meld u aan met uw tenantbeheerderaccount en controleer uw [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.</span><span class="sxs-lookup"><span data-stu-id="b3634-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="b3634-107">De Teams-toepassing verwijderen en opnieuw installeren (koppeling)</span><span class="sxs-lookup"><span data-stu-id="b3634-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="b3634-108">Blader naar de map %appdata%\Microsoft\teams\ op uw computer en verwijder alle bestanden in die adreslijst.</span><span class="sxs-lookup"><span data-stu-id="b3634-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="b3634-109">[Download en installeer de Teams-app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)en installeer Teams indien mogelijk als beheerder (klik met de rechtermuisknop op het Installatieprogramma van Teams en selecteer 'Uitvoeren als beheerder' indien beschikbaar).</span><span class="sxs-lookup"><span data-stu-id="b3634-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="b3634-110">Als uw Teams-client nog steeds vast loopt, kunt u het probleem dan reproduceren?</span><span class="sxs-lookup"><span data-stu-id="b3634-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="b3634-111">Zo ja:</span><span class="sxs-lookup"><span data-stu-id="b3634-111">If so:</span></span>

1. <span data-ttu-id="b3634-112">Gebruik de stappenrecorder om uw stappen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="b3634-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="b3634-113">Sluit ALLE overbodige of vertrouwelijke toepassingen.</span><span class="sxs-lookup"><span data-stu-id="b3634-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="b3634-114">Start de stappenrecorder en reproduceer het probleem terwijl u bent aangemeld met het betreffende gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="b3634-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="b3634-115">[Verzamel de teamslogboeken die de vastgelegde reprostappen vastleggen.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="b3634-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="b3634-116">**Opmerking:** Zorg ervoor dat u het aanmeldingsadres van de beïnvloede gebruiker vast legt.</span><span class="sxs-lookup"><span data-stu-id="b3634-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="b3634-117">Verzamel de dump- en/of foutemmergegevens (Windows).</span><span class="sxs-lookup"><span data-stu-id="b3634-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="b3634-118">Start Windows Powershell op de computer waar de crash plaatsvindt en voer de volgende opdrachten uit:</span><span class="sxs-lookup"><span data-stu-id="b3634-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="b3634-119">Voeg het bestand toe aan uw ondersteuningscase.</span><span class="sxs-lookup"><span data-stu-id="b3634-119">Attach the file to your support case.</span></span>
