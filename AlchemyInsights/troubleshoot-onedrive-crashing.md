---
title: Problemen met OneDrive-crashes oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748922"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="5c837-102">Problemen met OneDrive-crashes oplossen</span><span class="sxs-lookup"><span data-stu-id="5c837-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="5c837-103">Als OneDrive herhaaldelijk vastloopt, probeert u de volgende stappen voor het oplossen van problemen:</span><span class="sxs-lookup"><span data-stu-id="5c837-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="5c837-104">**Controleer of registersleutels niet zijn ingesteld:**</span><span class="sxs-lookup"><span data-stu-id="5c837-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="5c837-105">Navigeer met Registereditor naar HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="5c837-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="5c837-106">Als DisableFileSyncNGSC aanwezig is en is ingesteld op 1, opent u de toets en wijzigt u de waarde in 0.</span><span class="sxs-lookup"><span data-stu-id="5c837-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="5c837-107">OneDrive handmatig starten door naar het startscherm te gaan</span><span class="sxs-lookup"><span data-stu-id="5c837-107">Manually launch OneDrive by going to Start</span></span> ![Op de Windows-toets drukken](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="5c837-109">typ OneDrive in het zoekvak en klik op de OneDrive-bureaubladapp.</span><span class="sxs-lookup"><span data-stu-id="5c837-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="5c837-110">**OneDrive opnieuw instellen:**</span><span class="sxs-lookup"><span data-stu-id="5c837-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="5c837-111">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="5c837-111">Notes:</span></span>

- <span data-ttu-id="5c837-112">Het opnieuw instellen van OneDrive verbreekt al uw bestaande synchronisatieverbindingen (inclusief uw persoonlijke OneDrive als deze is ingesteld).</span><span class="sxs-lookup"><span data-stu-id="5c837-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="5c837-113">U verliest geen bestanden of gegevens door OneDrive opnieuw in te stellen op uw computer.</span><span class="sxs-lookup"><span data-stu-id="5c837-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="5c837-114">**OneDrive opnieuw instellen:**</span><span class="sxs-lookup"><span data-stu-id="5c837-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="5c837-115">Open een dialoogvenster Uitvoeren door op Windows-toets en R te drukken.</span><span class="sxs-lookup"><span data-stu-id="5c837-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="5c837-116">Typ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset en druk op OK.</span><span class="sxs-lookup"><span data-stu-id="5c837-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="5c837-117">Een opdrachtvenster kan kort worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="5c837-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="5c837-118">OneDrive handmatig starten door naar het startscherm te gaan</span><span class="sxs-lookup"><span data-stu-id="5c837-118">Manually launch OneDrive by going to Start</span></span> ![Op de Windows-toets drukken](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="5c837-120">typ OneDrive in het zoekvak en klik op de OneDrive-bureaubladapp.</span><span class="sxs-lookup"><span data-stu-id="5c837-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="5c837-121">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="5c837-121">Notes:</span></span>

- <span data-ttu-id="5c837-122">Als u ervoor had gekozen om slechts enkele mappen te synchroniseren voordat de reset, moet u dat opnieuw doen zodra de synchronisatie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="5c837-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="5c837-123">Lees [Welke OneDrive-mappen u wilt synchroniseren met uw computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)voor meer   informatie.</span><span class="sxs-lookup"><span data-stu-id="5c837-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="5c837-124">U moet dit voltooien voor uw persoonlijke OneDrive en OneDrive voor Bedrijven.</span><span class="sxs-lookup"><span data-stu-id="5c837-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>