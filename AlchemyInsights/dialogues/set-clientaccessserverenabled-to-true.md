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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523831"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="81bc9-102">ClientAccessServerEnabled instellen op Waar</span><span class="sxs-lookup"><span data-stu-id="81bc9-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="81bc9-103">Als u een versleuteld e-mailbericht niet kunt openen en in plaats daarvan een **rpmsg-bijlage** kunt zien, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="81bc9-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="81bc9-104">Verbinding maken met Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="81bc9-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="81bc9-105">Als u verbinding wilt maken met Exchange Online PowerShell, moet u zich aanmelden met een globale beheerder of een Exchange-beheerdersaccount.</span><span class="sxs-lookup"><span data-stu-id="81bc9-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="81bc9-106">a.</span><span class="sxs-lookup"><span data-stu-id="81bc9-106">a.</span></span> <span data-ttu-id="81bc9-107">Open Windows PowerShell en voer de volgende opdracht uit: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="81bc9-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="81bc9-108">b.</span><span class="sxs-lookup"><span data-stu-id="81bc9-108">b.</span></span> <span data-ttu-id="81bc9-109">Voer in **het dialoogvenster Referentieaanvraag** voor Windows PowerShell uw werk- of schoolaccount en wachtwoord in, c.</span><span class="sxs-lookup"><span data-stu-id="81bc9-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="81bc9-110">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="81bc9-110">Click **OK**.</span></span> 

2. <span data-ttu-id="81bc9-111">Voer de volgende opdracht uit om een nieuwe sessie te maken:</span><span class="sxs-lookup"><span data-stu-id="81bc9-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="81bc9-112">a.</span><span class="sxs-lookup"><span data-stu-id="81bc9-112">a.</span></span> <span data-ttu-id="81bc9-113">Voer de volgende opdracht uit:</span><span class="sxs-lookup"><span data-stu-id="81bc9-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="81bc9-114">Opdracht `Get-IRMConfiguration` Uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="81bc9-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="81bc9-115">Controleer de **instelling ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="81bc9-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="81bc9-116">a.</span><span class="sxs-lookup"><span data-stu-id="81bc9-116">a.</span></span> <span data-ttu-id="81bc9-117">Als **ClientAccessServerEnabled** is ingesteld op **Onwaar,** moet u de volgende cmdlet uitvoeren: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="81bc9-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="81bc9-118">Sluit uw PowerShell-sessie altijd met de volgende opdracht: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="81bc9-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="81bc9-119">Zie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="81bc9-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

