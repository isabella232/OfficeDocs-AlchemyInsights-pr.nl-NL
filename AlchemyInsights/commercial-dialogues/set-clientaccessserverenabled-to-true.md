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
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="085e2-102">ClientAccessServerEnabled instellen op Waar</span><span class="sxs-lookup"><span data-stu-id="085e2-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="085e2-103">Als u een versleuteld e-mailbericht niet kunt openen en in plaats daarvan een **rpmsg-bijlage** kunt zien, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="085e2-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="085e2-104">Verbinding maken met Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="085e2-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="085e2-105">Als u verbinding wilt maken met Exchange Online PowerShell, moet u zich aanmelden met een globale beheerder of Exchange-beheerdersaccount.</span><span class="sxs-lookup"><span data-stu-id="085e2-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="085e2-106">a.</span><span class="sxs-lookup"><span data-stu-id="085e2-106">a.</span></span> <span data-ttu-id="085e2-107">Open Windows PowerShell en voer de volgende opdracht uit: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="085e2-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="085e2-108">b.</span><span class="sxs-lookup"><span data-stu-id="085e2-108">b.</span></span> <span data-ttu-id="085e2-109">Voer in het dialoogvenster Aanmeldingsaanvraag voor **Windows PowerShell** uw werk- of schoolaccount en wachtwoord in, c.</span><span class="sxs-lookup"><span data-stu-id="085e2-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="085e2-110">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="085e2-110">Click **OK**.</span></span> 

2. <span data-ttu-id="085e2-111">Voer de volgende opdracht uit om een nieuwe sessie te maken:</span><span class="sxs-lookup"><span data-stu-id="085e2-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="085e2-112">a.</span><span class="sxs-lookup"><span data-stu-id="085e2-112">a.</span></span> <span data-ttu-id="085e2-113">Voer de volgende opdracht uit:</span><span class="sxs-lookup"><span data-stu-id="085e2-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="085e2-114">Voer `Get-IRMConfiguration` de opdracht uit.</span><span class="sxs-lookup"><span data-stu-id="085e2-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="085e2-115">Controleer de **instelling ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="085e2-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="085e2-116">a.</span><span class="sxs-lookup"><span data-stu-id="085e2-116">a.</span></span> <span data-ttu-id="085e2-117">Voer de volgende cmdlet uit als de instelling **ClientAccessServerEnabled** is ingesteld op **Onwaar:**`Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="085e2-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="085e2-118">Sluit uw powershell-sessie altijd met de volgende opdracht: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="085e2-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="085e2-119">Zie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="085e2-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

