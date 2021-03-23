---
title: Schijfruimte vrij maken in Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035666"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a7849-102">Schijfruimte vrij maken in Windows 10</span><span class="sxs-lookup"><span data-stu-id="a7849-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a7849-103">Hier zijn twee opties om schijfruimte vrij te maken in Windows:</span><span class="sxs-lookup"><span data-stu-id="a7849-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a7849-104">Schijfruimte vrij maken in Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a7849-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a7849-105">Ruimte vrij maken voor Windows 10-updates met een extern opslagapparaat.</span><span class="sxs-lookup"><span data-stu-id="a7849-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a7849-106">Als u na het gebruik van Schijfopruiming nog steeds weinig schijfruimte hebt, is het mogelijk dat de map Temp snel wordt gevuld met toepassingsbestanden (.appx) die door Microsoft Store worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="a7849-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a7849-107">U kunt dit probleem oplossen door de Store opnieuw in te stellen, de Store-cache te wissen en vervolgens de probleemoplosser voor Windows Update uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="a7849-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a7849-108">Zorg ervoor dat de Microsoft Store is gesloten voordat u verder gaat met deze stappen.</span><span class="sxs-lookup"><span data-stu-id="a7849-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a7849-109">**Stap 1: Microsoft Store opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="a7849-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a7849-110">**Opmerking** Hiermee worden de app-gegevens op het apparaat definitief verwijderd, inclusief uw voorkeuren en aanmeldingsgegevens.</span><span class="sxs-lookup"><span data-stu-id="a7849-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a7849-111">Selecteer **Instellingen instellingen**  >  **apps** starten  >  **Apps**&  >  **functies**.</span><span class="sxs-lookup"><span data-stu-id="a7849-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a7849-112">Zoek en selecteer Microsoft Store in de lijst met apps.</span><span class="sxs-lookup"><span data-stu-id="a7849-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a7849-113">Selecteer **Geavanceerde opties.**</span><span class="sxs-lookup"><span data-stu-id="a7849-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a7849-114">Schuif omlaag en selecteer **Opnieuw instellen** en bevestig **opnieuw instellen.**</span><span class="sxs-lookup"><span data-stu-id="a7849-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a7849-115">**Stap 2: De Microsoft Store-cache wissen**</span><span class="sxs-lookup"><span data-stu-id="a7849-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a7849-116">Druk op de Windows-logotoets + R om het dialoogvenster Uitvoeren te openen.</span><span class="sxs-lookup"><span data-stu-id="a7849-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a7849-117">Typ wsreset.exe en selecteer **OK.**</span><span class="sxs-lookup"><span data-stu-id="a7849-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a7849-118">Er wordt een leeg venster met opdrachtprompt geopend.</span><span class="sxs-lookup"><span data-stu-id="a7849-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a7849-119">Na ongeveer 10 seconden wordt het venster gesloten en wordt de Store automatisch geopend.</span><span class="sxs-lookup"><span data-stu-id="a7849-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a7849-120">**Stap 3: Windows Update opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="a7849-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a7849-121">Selecteer **Instellingen bijwerken**  >  **starten** om &  >  **beveiligingsproblemen op te**  >  **lossen.**</span><span class="sxs-lookup"><span data-stu-id="a7849-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a7849-122">Schuif omlaag en selecteer **Windows Update** in de lijst en selecteer **De probleemoplosser uitvoeren.**</span><span class="sxs-lookup"><span data-stu-id="a7849-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a7849-123">Start uw computer opnieuw op en controleer of u het probleem nog steeds ondervindt.</span><span class="sxs-lookup"><span data-stu-id="a7849-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

