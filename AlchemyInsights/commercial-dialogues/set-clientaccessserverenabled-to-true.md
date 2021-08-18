---
title: ClientAccessServerEnabled instellen op Waar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320351"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled instellen op Waar

Als u een versleuteld e-mailbericht niet kunt openen en in plaats daarvan een **rpmsg-bijlage** kunt zien, voert u de volgende stappen uit:

1. Verbinding maken met Exchange Online PowerShell.

    **Opmerking:** Als u verbinding wilt maken met Exchange Online PowerShell, moet u zich aanmelden met een globale beheerder of een Exchange beheerdersaccount.

   a. Open Windows PowerShell en voer de volgende opdracht uit:`$UserCredential = Get-Credential`
   b. Voer in **Windows PowerShell dialoogvenster Aanvraag** voor referenties uw werk- of schoolaccount en wachtwoord in, c. Klik op **OK**. 

2. Voer de volgende opdracht uit om een nieuwe sessie te maken:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Voer de volgende opdracht uit:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Voer `Get-IRMConfiguration` de opdracht uit.

4. Controleer de **instelling ClientAccessServerEnabled.** 

    a. Voer de volgende cmdlet uit als de instelling **ClientAccessServerEnabled** is ingesteld op **Onwaar:**`Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tip:** Sluit uw powershell-sessie altijd met de volgende opdracht: `Remove-PSSession $Session`

Zie voor meer informatie [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

