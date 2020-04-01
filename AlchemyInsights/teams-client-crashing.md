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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030588"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="0521a-102">Teams-cliënt crasht?</span><span class="sxs-lookup"><span data-stu-id="0521a-102">Teams client crashing?</span></span>

<span data-ttu-id="0521a-103">Als uw Teams-client crasht, probeer dan het volgende:</span><span class="sxs-lookup"><span data-stu-id="0521a-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0521a-104">Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0521a-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0521a-105">Zorg ervoor dat alle [ URL's en adresbereiken van Office 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.</span><span class="sxs-lookup"><span data-stu-id="0521a-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0521a-106">Log in met uw beheerdersaccount en controleer uw [ Servicestatusdashboard ](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen storing of serviceafname is.</span><span class="sxs-lookup"><span data-stu-id="0521a-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="0521a-107">Als laatste stap kunt u proberen de cache van uw Teams-cliënt te wissen:</span><span class="sxs-lookup"><span data-stu-id="0521a-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="0521a-108">Sluit de Microsoft Teams-desktopclient volledig af.</span><span class="sxs-lookup"><span data-stu-id="0521a-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="0521a-109">U kunt met de rechtermuisknop op \*\* Teams \*\* klikken in het pictogramvak en op \*\* Afsluiten \*\* klikken, of Taakbeheer uitvoeren en het proces volledig beëindigen.</span><span class="sxs-lookup"><span data-stu-id="0521a-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="0521a-110">Ga naar Verkenner en typ % appdata% \Microsoft\teams in.</span><span class="sxs-lookup"><span data-stu-id="0521a-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="0521a-111">Eenmaal in de directory ziet u enkele van de volgende mappen:</span><span class="sxs-lookup"><span data-stu-id="0521a-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="0521a-112">Ga vanuit \*\* Application Cache \*\* naar Cache en verwijder alle bestanden op de Cache-locatie: % appdata%\Microsoft\teams\applicationcache\cache.</span><span class="sxs-lookup"><span data-stu-id="0521a-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="0521a-113">Verwijder vanuit \*\* Blob_storage \*\* alle bestanden: % appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="0521a-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="0521a-114">Verwijder vanuit \*\* Cache \*\* alle bestanden: % appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="0521a-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="0521a-115">Verwijder vanuit \*\* databases \*\* alle bestanden: % appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="0521a-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="0521a-116">Verwijder vanuit \*\* GPUCache \*\* alle bestanden: % appdata%\Microsoft\teams\GPUCache.</span><span class="sxs-lookup"><span data-stu-id="0521a-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="0521a-117">Verwijder vanuit \*\* IndexedDB \*\* alle bestanden: % appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="0521a-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="0521a-118">Verwijder vanuit \*\*Local Storage \*\* alle bestanden: % appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="0521a-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="0521a-119">Verwijder vanuit \*\*tmp \*\* alle bestanden: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="0521a-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="0521a-120">Start uw Teams-cliënt opnieuw op.</span><span class="sxs-lookup"><span data-stu-id="0521a-120">Restart your Teams client.</span></span>
