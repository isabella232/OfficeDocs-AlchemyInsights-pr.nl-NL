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
# <a name="troubleshoot-onedrive-crashes"></a>Problemen met OneDrive-crashes oplossen

Als OneDrive herhaaldelijk vastloopt, probeert u de volgende stappen voor het oplossen van problemen:

**Controleer of registersleutels niet zijn ingesteld:**

1. Navigeer met Registereditor naar HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Als DisableFileSyncNGSC aanwezig is en is ingesteld op 1, opent u de toets en wijzigt u de waarde in 0.
3. OneDrive handmatig starten door naar het startscherm te gaan ![Op de Windows-toets drukken](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)typ OneDrive in het zoekvak en klik op de OneDrive-bureaubladapp.

**OneDrive opnieuw instellen:**

Opmerkingen:

- Het opnieuw instellen van OneDrive verbreekt al uw bestaande synchronisatieverbindingen (inclusief uw persoonlijke OneDrive als deze is ingesteld).
- U verliest geen bestanden of gegevens door OneDrive opnieuw in te stellen op uw computer.

**OneDrive opnieuw instellen:**

1. Open een dialoogvenster Uitvoeren door op Windows-toets en R te drukken.
2. Typ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset en druk op OK. Een opdrachtvenster kan kort worden weergegeven.
3. OneDrive handmatig starten door naar het startscherm te gaan ![Op de Windows-toets drukken](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)typ OneDrive in het zoekvak en klik op de OneDrive-bureaubladapp.

Opmerkingen:

- Als u ervoor had gekozen om slechts enkele mappen te synchroniseren voordat de reset, moet u dat opnieuw doen zodra de synchronisatie is voltooid. Lees [Welke OneDrive-mappen u wilt synchroniseren met uw computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)voor meer   informatie.
- U moet dit voltooien voor uw persoonlijke OneDrive en OneDrive voor Bedrijven.