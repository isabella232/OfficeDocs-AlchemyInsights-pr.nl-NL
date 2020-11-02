---
title: 0x8004de40-fout bij het starten van OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823017"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-fout bij het starten van OneDrive

Als u een foutmelding krijgt **0x8004de40** wanneer u zich aanmeldt bij OneDrive, start u de computer opnieuw op terwijl u verbinding hebt met het domein van uw werk of school. Als u deze foutmelding krijgt nadat u de computer opnieuw hebt opgestart, kunt u dit proberen wanneer u verbinding hebt met uw werk-of school domein:

1. Klik op Start en typ **cmd** of **Command prompt**  in het zoekvak, klik met de rechtermuisknop op de opdrachtprompt-app en selecteer  **als administrator uitvoeren** . Als u wordt gevraagd om een beheerderswachtwoord of een bevestiging, typt u het wachtwoord of klikt u op **toestaan** .  

2. Typ in het venster met de opdracht prompt de tekst **dsregcmd/Leave**  en wacht totdat de opdracht klaar is. Typ vervolgens **dsregcmd/join** en wacht tot de opdracht klaar is.
3. Start de computer opnieuw op.
