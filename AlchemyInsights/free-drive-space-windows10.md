---
title: Schijfruimte vrijmaken in Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505351"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="da058-102">Schijfruimte vrijmaken in Windows 10</span><span class="sxs-lookup"><span data-stu-id="da058-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="da058-103">Hier volgen twee opties voor het vrijmaken van schijfruimte in Windows:</span><span class="sxs-lookup"><span data-stu-id="da058-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="da058-104">Schijfruimte vrijmaken in Windows 10.</span><span class="sxs-lookup"><span data-stu-id="da058-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="da058-105">Schijfruimte vrijmaken voor Windows 10 updates met extern opslagapparaat.</span><span class="sxs-lookup"><span data-stu-id="da058-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="da058-106">Als je nog steeds weinig schijfruimte heeft na het gebruiken van Disk Cleanup is het mogelijk dat uw tijdelijke map snel vol geraakt met applicatiebestanden (.appx) die gebruikt worden door Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="da058-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="da058-107">Los dit probleem op de Store opnieuw in te stellen de cache van de Store te wissen en vervolgens de Windows Update probleemoplosser uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="da058-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="da058-108">Zorg ervoor dat Microsoft Store gesloten is voor je verder gaat met deze stappen.</span><span class="sxs-lookup"><span data-stu-id="da058-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="da058-109">**Stap 1: Microsoft Store opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="da058-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="da058-110">**Opmerking** Dit verwijdert de app-gegevens op dit apparaat permanent, inclusief je voorkeuren en aanmeldingsgegevens.</span><span class="sxs-lookup"><span data-stu-id="da058-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="da058-111">Selecteer **Start** > **Instellingen** > **Apps** > **Apps en functies**.</span><span class="sxs-lookup"><span data-stu-id="da058-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="da058-112">Vind en selecteer Microsoft Store in de lijst met apps.</span><span class="sxs-lookup"><span data-stu-id="da058-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="da058-113">Selecteer **Geavanceerde opties**.</span><span class="sxs-lookup"><span data-stu-id="da058-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="da058-114">Schuif naar beneden en selecteer **Opnieuw instellen** en vervolgens **Opnieuw instellen bevestigen**.</span><span class="sxs-lookup"><span data-stu-id="da058-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="da058-115">**Stap 2: de Microsoft Store cache verwijderen**</span><span class="sxs-lookup"><span data-stu-id="da058-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="da058-116">Druk op de Windows-logotoets + R om het dialoogvenster Uitvoeren te openen.</span><span class="sxs-lookup"><span data-stu-id="da058-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="da058-117">Typ in wsreset.exe en selecteer **Ok**.</span><span class="sxs-lookup"><span data-stu-id="da058-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="da058-118">Een lege opdrachtprompt wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="da058-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="da058-119">Na ongeveer 10 seconden wordt het venster gesloten en wordt de Store automatisch geopend.</span><span class="sxs-lookup"><span data-stu-id="da058-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="da058-120">**Stap 3: Windows update opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="da058-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="da058-121">Selecteer **Start** > **Instellingen** > **Updates en beveiliging** > **Probleemzoeker**.</span><span class="sxs-lookup"><span data-stu-id="da058-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="da058-122">Schuif naar beneden en kies **Windows update** uit de lijst en selecteer **Probleemzoeker uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="da058-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="da058-123">Start de computer opnieuw op en controleer of het probleem zich nog steeds voordoet.</span><span class="sxs-lookup"><span data-stu-id="da058-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

