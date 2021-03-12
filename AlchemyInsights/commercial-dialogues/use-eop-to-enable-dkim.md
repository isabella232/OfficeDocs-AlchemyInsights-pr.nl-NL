---
title: Exchange Online PowerShell gebruiken om DKIM in te stellen voor een specifiek domein
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744649"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Exchange Online PowerShell gebruiken om DKIM in te stellen voor een specifiek domein

Als u de DKIM DNS-records niet kunt maken in het beheercentrum, kunt u Exchange Online PowerShell gebruiken. 

Als u een DKIM DNS-record wilt maken met Exchange Online PowerShell, voert u de volgende stappen uit:

1. Open Windows PowerShell als beheerder en voer de volgende opdrachten uit in de beschreven volgorde:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Zie Verbinding maken met Exchange Online PowerShell als u problemen hebt met het maken van verbinding met Exchange Online [PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Voer de volgende opdracht uit wanneer u verbinding hebt met Exchange Online PowerShell:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Nadat de bovenstaande opdracht is uitgevoerd, kunt u de volgende opdracht uitvoeren om de Exchange Online PowerShell-sessie te beëindigen:

    `Remove-PSSession $Session` 



