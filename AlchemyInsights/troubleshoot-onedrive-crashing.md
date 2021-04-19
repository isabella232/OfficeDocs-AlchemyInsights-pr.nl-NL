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
# <a name="troubleshoot-onedrive-crashes"></a>Problemen met crashes in OneDrive oplossen

Als OneDrive herhaaldelijk vast loopt, kunt u de volgende stappen voor probleemoplossing proberen:

**Controleer of registersleutels niet zijn ingesteld:**

1. Navigeer met registereditor naar HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Als DisableFileSyncNGSC aanwezig is en is ingesteld op 1, opent u de sleutel en wijzigt u de waarde in 0.
3. OneDrive handmatig starten door naar Start te gaan ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), typ OneDrive in het zoekvak en klik vervolgens op de bureaublad-app van OneDrive.

**OneDrive opnieuw instellen:**

Opmerkingen:

- Als u OneDrive opnieuw in stelt, worden al uw bestaande synchronisatieverbindingen verbroken (inclusief uw persoonlijke OneDrive indien ingesteld).
- U raakt geen bestanden of gegevens kwijt door OneDrive opnieuw in te zetten op uw computer.

**OneDrive opnieuw instellen:**

1. Open een dialoogvenster Uitvoeren door op Windows-toets en R te drukken.
2. Typ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset en druk op OK. Een opdrachtvenster kan kort worden weergegeven.
3. OneDrive handmatig starten door naar Start te gaan ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), typ OneDrive in het zoekvak en klik vervolgens op de bureaublad-app van OneDrive.

Opmerkingen:

- Als u ervoor had gekozen om slechts enkele mappen te synchroniseren vóór de reset, moet u dit opnieuw doen nadat de synchronisatie is voltooid. Lees [Kiezen welke OneDrive-mappen u wilt synchroniseren met uw computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)voor meer   informatie.
- U moet dit voltooien voor uw persoonlijke OneDrive en OneDrive voor Bedrijven.