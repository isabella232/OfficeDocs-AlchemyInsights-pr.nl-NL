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
# <a name="teams-client-crashing"></a><span data-ttu-id="f6c05-102">Teams-cliënt crasht?</span><span class="sxs-lookup"><span data-stu-id="f6c05-102">Teams client crashing?</span></span>

<span data-ttu-id="f6c05-103">Als uw Teams-client crasht, probeer dan het volgende:</span><span class="sxs-lookup"><span data-stu-id="f6c05-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f6c05-104">Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f6c05-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f6c05-105">Zorg ervoor dat alle [Microsoft 365-URL's en adresbereiken](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.</span><span class="sxs-lookup"><span data-stu-id="f6c05-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f6c05-106">Meld u aan met uw tenantadmin-account en controleer uw [dashboard servicestatus](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen uitval of servicedegradatie bestaat.</span><span class="sxs-lookup"><span data-stu-id="f6c05-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="f6c05-107">De Teams-toepassing verwijderen en opnieuw installeren (koppeling)</span><span class="sxs-lookup"><span data-stu-id="f6c05-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="f6c05-108">Blader naar de map %appdata%\Microsoft\teams\ op uw computer en verwijder alle bestanden in die map.</span><span class="sxs-lookup"><span data-stu-id="f6c05-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="f6c05-109">[Download en installeer de Teams-app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)en installeer teams indien mogelijk als beheerder (klik met de rechtermuisknop op het installatieprogramma Teams en selecteer 'Uitvoeren als beheerder' indien beschikbaar).</span><span class="sxs-lookup"><span data-stu-id="f6c05-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="f6c05-110">Als uw Teams-client nog steeds crasht, u het probleem reproduceren?</span><span class="sxs-lookup"><span data-stu-id="f6c05-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="f6c05-111">Zo ja:</span><span class="sxs-lookup"><span data-stu-id="f6c05-111">If so:</span></span>

1. <span data-ttu-id="f6c05-112">Gebruik de Steps Recorder om uw stappen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="f6c05-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f6c05-113">Sluit ALLE onnodige of vertrouwelijke toepassingen.</span><span class="sxs-lookup"><span data-stu-id="f6c05-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f6c05-114">Start de Steps Recorder en reproduceren het probleem terwijl ingelogd met de getroffen gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="f6c05-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="f6c05-115">[Verzamel de teams logs die de opgenomen repro stappen vast te leggen](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="f6c05-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="f6c05-116">**Opmerking:** zorg ervoor dat u het aanmeldingsadres van de getroffen gebruiker vastlegt.</span><span class="sxs-lookup"><span data-stu-id="f6c05-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="f6c05-117">Verzamel de dump- en/of foutbucket-informatie (Windows).</span><span class="sxs-lookup"><span data-stu-id="f6c05-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="f6c05-118">Start Windows Powershell op de machine waar de crash plaatsvindt en voer de volgende opdrachten uit:</span><span class="sxs-lookup"><span data-stu-id="f6c05-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="f6c05-119">Voeg het bestand toe aan uw ondersteuningsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="f6c05-119">Attach the file to your support case.</span></span>
