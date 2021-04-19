---
title: Problemen met crashes in OneDrive oplossen
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826194"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="8ab71-102">Problemen met crashes in OneDrive oplossen</span><span class="sxs-lookup"><span data-stu-id="8ab71-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="8ab71-103">Als OneDrive herhaaldelijk vast loopt, kunt u de volgende stappen voor probleemoplossing proberen:</span><span class="sxs-lookup"><span data-stu-id="8ab71-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="8ab71-104">**Controleer of registersleutels niet zijn ingesteld:**</span><span class="sxs-lookup"><span data-stu-id="8ab71-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="8ab71-105">Navigeer met registereditor naar HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="8ab71-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="8ab71-106">Als DisableFileSyncNGSC aanwezig is en is ingesteld op 1, opent u de sleutel en wijzigt u de waarde in 0.</span><span class="sxs-lookup"><span data-stu-id="8ab71-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="8ab71-107">OneDrive handmatig starten door naar Start te gaan</span><span class="sxs-lookup"><span data-stu-id="8ab71-107">Manually launch OneDrive by going to Start</span></span> ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8ab71-109">, typ OneDrive in het zoekvak en klik vervolgens op de bureaublad-app van OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8ab71-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8ab71-110">**OneDrive opnieuw instellen:**</span><span class="sxs-lookup"><span data-stu-id="8ab71-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="8ab71-111">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="8ab71-111">Notes:</span></span>

- <span data-ttu-id="8ab71-112">Als u OneDrive opnieuw in stelt, worden al uw bestaande synchronisatieverbindingen verbroken (inclusief uw persoonlijke OneDrive indien ingesteld).</span><span class="sxs-lookup"><span data-stu-id="8ab71-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="8ab71-113">U raakt geen bestanden of gegevens kwijt door OneDrive opnieuw in te zetten op uw computer.</span><span class="sxs-lookup"><span data-stu-id="8ab71-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="8ab71-114">**OneDrive opnieuw instellen:**</span><span class="sxs-lookup"><span data-stu-id="8ab71-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="8ab71-115">Open een dialoogvenster Uitvoeren door op Windows-toets en R te drukken.</span><span class="sxs-lookup"><span data-stu-id="8ab71-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="8ab71-116">Typ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset en druk op OK.</span><span class="sxs-lookup"><span data-stu-id="8ab71-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="8ab71-117">Een opdrachtvenster kan kort worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="8ab71-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="8ab71-118">OneDrive handmatig starten door naar Start te gaan</span><span class="sxs-lookup"><span data-stu-id="8ab71-118">Manually launch OneDrive by going to Start</span></span> ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8ab71-120">, typ OneDrive in het zoekvak en klik vervolgens op de bureaublad-app van OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8ab71-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8ab71-121">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="8ab71-121">Notes:</span></span>

- <span data-ttu-id="8ab71-122">Als u ervoor had gekozen om slechts enkele mappen te synchroniseren vóór de reset, moet u dit opnieuw doen nadat de synchronisatie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="8ab71-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="8ab71-123">Lees [Kiezen welke OneDrive-mappen u wilt synchroniseren met uw computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)voor meer   informatie.</span><span class="sxs-lookup"><span data-stu-id="8ab71-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="8ab71-124">U moet dit voltooien voor uw persoonlijke OneDrive en OneDrive voor Bedrijven.</span><span class="sxs-lookup"><span data-stu-id="8ab71-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>