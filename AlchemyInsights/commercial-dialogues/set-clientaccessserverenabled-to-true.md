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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744706"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled instellen op Waar

Als u een versleuteld e-mailbericht niet kunt openen en in plaats daarvan een **rpmsg-bijlage** kunt zien, voert u de volgende stappen uit:

1. Verbinding maken met Exchange Online PowerShell.

> [!NOTE]
> Als u verbinding wilt maken met Exchange Online PowerShell, moet u zich aanmelden met een globale beheerder of Exchange-beheerdersaccount.

   a. Open Windows PowerShell en voer de volgende opdracht uit: `$UserCredential = Get-Credential`
b. Voer in het dialoogvenster Aanmeldingsaanvraag voor **Windows PowerShell** uw werk- of schoolaccount en wachtwoord in, c. Klik op **OK**. 

2. Voer de volgende opdracht uit om een nieuwe sessie te maken:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Voer de volgende opdracht uit:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Voer `Get-IRMConfiguration` de opdracht uit.

4. Controleer de **instelling ClientAccessServerEnabled.** 

    a. Voer de volgende cmdlet uit als de instelling **ClientAccessServerEnabled** is ingesteld op **Onwaar:**`Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sluit uw powershell-sessie altijd met de volgende opdracht: `Remove-PSSession $Session`

Zie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)voor meer informatie.

