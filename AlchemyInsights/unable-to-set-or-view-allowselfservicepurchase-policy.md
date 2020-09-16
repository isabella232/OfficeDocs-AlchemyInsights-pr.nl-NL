---
title: Kan het AllowSelfServicePurchase-beleid niet instellen of weergeven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735194"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="f8bc1-102">Kan het AllowSelfServicePurchase-beleid niet instellen of weergeven</span><span class="sxs-lookup"><span data-stu-id="f8bc1-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="f8bc1-103">Wanneer u probeert het AllowSelfServicePurchase-beleid in te stellen of weer te geven, wordt het volgende foutbericht weergegeven:</span><span class="sxs-lookup"><span data-stu-id="f8bc1-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="f8bc1-104">*HandleError: kan geen productbeleid ophalen met PolicyId ' AllowSelfServicePurchase ', ErrorMessage-de onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden bij het verzenden.*</span><span class="sxs-lookup"><span data-stu-id="f8bc1-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="f8bc1-105">Dit kan zijn vanwege een oudere versie van TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="f8bc1-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="f8bc1-106">U moet TLS 1,2 of hoger gebruiken om verbinding te maken met de MSCommerce-service.</span><span class="sxs-lookup"><span data-stu-id="f8bc1-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="f8bc1-107">Voer de volgende stappen uit om het TLS-protocol in te stellen op 1,2, Controleer en probeer het opnieuw.</span><span class="sxs-lookup"><span data-stu-id="f8bc1-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="f8bc1-108">Bij de PowerShell-opdrachtprompt (PS C: \) Voer de volgende opdracht in om het TLS-protocol in te stellen op versie 1,2:</span><span class="sxs-lookup"><span data-stu-id="f8bc1-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="f8bc1-109">Controleer de TLS-protocol (s) die u gebruikt, met de volgende opdracht:</span><span class="sxs-lookup"><span data-stu-id="f8bc1-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="f8bc1-110">Voer de opdrachten voor het uitvoeren of bijwerken naar wens opnieuw.</span><span class="sxs-lookup"><span data-stu-id="f8bc1-110">Retry the Get or Update commands as needed.</span></span>

