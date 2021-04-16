---
title: Exchange PowerShell en de afschaffing van basisverificatie
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813467"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="45913-102">Exchange PowerShell en de afschaffing van basisverificatie</span><span class="sxs-lookup"><span data-stu-id="45913-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="45913-103">Als u de meest recente informatie wilt over het maken van verbinding met Exchange Online PowerShell zonder het gebruik van basisverificatie, [gaat u hierheen](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="45913-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="45913-104">De Windows PowerShell V2 module gebruikt geen basisverificatie.</span><span class="sxs-lookup"><span data-stu-id="45913-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="45913-105">Houd er rekening mee dat Basisverificatie nog steeds moet zijn ingeschakeld op uw clientcomputer.</span><span class="sxs-lookup"><span data-stu-id="45913-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="45913-106">De nieuwe PowerShell V2-module gebruikt moderne verificatie om een verbinding tot stand te brengen voor het inschakelen van alle REST V2-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="45913-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="45913-107">Naast de V2-cmdlets krijgt u ook toegang tot oudere RPS-cmdlets (Remote PowerShell) waarvoor een Remote PowerShell-sessie nodig is.</span><span class="sxs-lookup"><span data-stu-id="45913-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="45913-108">Voor het tot stand brengen van een RPS-sessie op Windows-apparaten moet WinRM BasicAuth zijn ingeschakeld op de clientcomputer, ook al gebruikt de module het mechanisme van moderne verificatie om de service te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="45913-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="45913-109">De WinRM-basisverificatiepijplijn wordt gebruikt voor het transport van tokens van moderne verificatie.</span><span class="sxs-lookup"><span data-stu-id="45913-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="45913-110">Als WinRM-basisverificatie is uitgeschakeld op de clientcomputer blijven de nieuwe V2-cmdlets werken (maar de oudere RPS-cmdlets niet).</span><span class="sxs-lookup"><span data-stu-id="45913-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
