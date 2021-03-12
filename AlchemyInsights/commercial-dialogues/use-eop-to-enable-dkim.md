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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="51e2f-102">Exchange Online PowerShell gebruiken om DKIM in te stellen voor een specifiek domein</span><span class="sxs-lookup"><span data-stu-id="51e2f-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="51e2f-103">Als u de DKIM DNS-records niet kunt maken in het beheercentrum, kunt u Exchange Online PowerShell gebruiken.</span><span class="sxs-lookup"><span data-stu-id="51e2f-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="51e2f-104">Als u een DKIM DNS-record wilt maken met Exchange Online PowerShell, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="51e2f-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="51e2f-105">Open Windows PowerShell als beheerder en voer de volgende opdrachten uit in de beschreven volgorde:</span><span class="sxs-lookup"><span data-stu-id="51e2f-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="51e2f-106">a.</span><span class="sxs-lookup"><span data-stu-id="51e2f-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="51e2f-107">b.</span><span class="sxs-lookup"><span data-stu-id="51e2f-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="51e2f-108">c.</span><span class="sxs-lookup"><span data-stu-id="51e2f-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="51e2f-109">Zie Verbinding maken met Exchange Online PowerShell als u problemen hebt met het maken van verbinding met Exchange Online [PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="51e2f-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="51e2f-110">Voer de volgende opdracht uit wanneer u verbinding hebt met Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="51e2f-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="51e2f-111">Nadat de bovenstaande opdracht is uitgevoerd, kunt u de volgende opdracht uitvoeren om de Exchange Online PowerShell-sessie te beëindigen:</span><span class="sxs-lookup"><span data-stu-id="51e2f-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



