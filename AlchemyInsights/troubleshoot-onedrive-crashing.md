---
title: Problemen met OneDrive crashes oplossen
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921002"
---
# <a name="troubleshoot-onedrive-crashes"></a>Problemen met OneDrive crashes oplossen

Als OneDrive herhaaldelijk vast loopt, kunt u de volgende stappen voor het oplossen van problemen proberen:

**Controleer of registersleutels niet zijn ingesteld:**

1. Navigeer met registereditor naar HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Als DisableFileSyncNGSC aanwezig is en is ingesteld op 1, opent u de sleutel en wijzigt u de waarde in 0.
3. Start de OneDrive handmatig door naar Start te gaan ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), typ OneDrive in het zoekvak en klik vervolgens op de OneDrive bureaublad-app.

**De OneDrive:**

Opmerkingen:

- Als u de OneDrive, worden al uw bestaande synchronisatieverbindingen (inclusief uw persoonlijke OneDrive indien ingesteld) verbroken.
- U verliest geen bestanden of gegevens door het opnieuw instellen van OneDrive op uw computer.

**U kunt de OneDrive:**

1. Open een dialoogvenster Uitvoeren door op Windows en R.
2. Typ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset en druk op OK. Een opdrachtvenster kan kort worden weergegeven.
3. Start de OneDrive handmatig door naar Start te gaan ![Druk op de Windows-toets](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), typ OneDrive in het zoekvak en klik vervolgens op de OneDrive bureaublad-app.

Opmerkingen:

- Als u ervoor had gekozen om slechts enkele mappen te synchroniseren vóór de reset, moet u dit opnieuw doen nadat de synchronisatie is voltooid. Lees [Kiezen welke OneDrive wilt synchroniseren met uw computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)voor meer   informatie.
- U moet dit voltooien voor uw persoonlijke OneDrive en OneDrive voor Bedrijven.