---
title: Exchange PowerShell en de afschaffing van basisverificatie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015684"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="50a7d-102">Exchange PowerShell en de afschaffing van basisverificatie</span><span class="sxs-lookup"><span data-stu-id="50a7d-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="50a7d-103">Als u de meest recente informatie wilt over het maken van verbinding met Exchange Online PowerShell zonder het gebruik van basisverificatie, [gaat u hierheen](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="50a7d-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="50a7d-104">Houd er rekening mee dat Basisverificatie nog steeds moet zijn ingeschakeld op uw clientcomputer.</span><span class="sxs-lookup"><span data-stu-id="50a7d-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="50a7d-105">De nieuwe PowerShell V2-module gebruikt moderne verificatie om een verbinding tot stand te brengen voor het inschakelen van alle REST V2-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="50a7d-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="50a7d-106">Naast de V2-cmdlets krijgt u ook toegang tot oudere RPS-cmdlets (Remote PowerShell) waarvoor een Remote PowerShell-sessie nodig is.</span><span class="sxs-lookup"><span data-stu-id="50a7d-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="50a7d-107">Voor het tot stand brengen van een RPS-sessie op Windows-apparaten moet WinRM BasicAuth zijn ingeschakeld op de clientcomputer, ook al gebruikt de module het mechanisme van moderne verificatie om de service te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="50a7d-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="50a7d-108">De WinRM-basisverificatiepijplijn wordt gebruikt voor het transport van tokens van moderne verificatie.</span><span class="sxs-lookup"><span data-stu-id="50a7d-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="50a7d-109">Als WinRM-basisverificatie is uitgeschakeld op de clientcomputer blijven de nieuwe V2-cmdlets werken (maar de oudere RPS-cmdlets niet).</span><span class="sxs-lookup"><span data-stu-id="50a7d-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
