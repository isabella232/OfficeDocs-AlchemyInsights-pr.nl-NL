---
title: 0x8004de40 fout bij het starten van OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946574"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 fout bij het starten van OneDrive

Als u een foutmelding **0x8004de40** bij het aanmelden bij OneDrive, start u de computer opnieuw op terwijl deze is verbonden met uw werk- of schooldomein. Als u deze fout ontvangt na het opnieuw opstarten, probeert u dit terwijl u verbonden bent met uw werk- of schooldomein:

1. Klik op Start en typ **cmd** of **opdrachtprompt** in het zoekvak, klik met de rechtermuisknop op de opdrachtprompt-app en selecteer **Als beheerder uitvoeren.** Als u wordt gevraagd om een beheerderswachtwoord of om een bevestiging, typt u het wachtwoord of klikt u op **Toestaan.**  

2. Typ in het venster Opdrachtprompt **dsregcmd /leave**  en wacht totdat de opdracht is voltooid. Typ **vervolgens dsregcmd /join** en wacht totdat de opdracht is voltooid.
3. Start de computer opnieuw op.
