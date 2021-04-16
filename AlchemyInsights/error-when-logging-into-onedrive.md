---
title: 0x8004de40 bij het starten van OneDrive
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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813647"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 bij het starten van OneDrive

Als u een foutmelding **0x8004de40** wanneer u zich bij OneDrive aanmeldt, start u de computer opnieuw op terwijl deze is verbonden met uw werk- of schooldomein. Als u deze fout ontvangt na het opnieuw opstarten, probeert u dit terwijl u verbonden bent met uw werk- of schooldomein:

1. Klik op Start en typ **cmd** of **opdrachtprompt** in het zoekvak, klik met de rechtermuisknop op de opdrachtprompt-app en selecteer **Als beheerder uitvoeren.** Als u wordt gevraagd om een beheerderswachtwoord of om een bevestiging, typt u het wachtwoord of klikt u op **Toestaan.**  

2. Typ in het venster Opdrachtprompt **dsregcmd /leave**  en wacht totdat de opdracht is voltooid. Typ **vervolgens dsregcmd /join** en wacht totdat de opdracht is voltooid.
3. Start de computer opnieuw op.
