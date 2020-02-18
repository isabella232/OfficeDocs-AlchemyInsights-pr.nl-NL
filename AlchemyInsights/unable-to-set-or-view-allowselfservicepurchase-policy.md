---
title: Kan het AllowSelfServicePurchase-beleid niet instellen of bekijken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091686"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="cf11f-102">Kan het AllowSelfServicePurchase-beleid niet instellen of bekijken</span><span class="sxs-lookup"><span data-stu-id="cf11f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="cf11f-103">Wanneer u het allowselfservice-aankoopbeleid probeert in te stellen of weer te geven, ontvangt u het volgende foutbericht:</span><span class="sxs-lookup"><span data-stu-id="cf11f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="cf11f-104">*HandleError : Kan het productbeleid niet ophalen met PolicyId 'AllowSelfServicePurchase', ErrorMessage - De onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden op een verzenden.*</span><span class="sxs-lookup"><span data-stu-id="cf11f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="cf11f-105">Dit kan te wijten zijn aan een oudere versie van Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="cf11f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="cf11f-106">Als u de MSCommerce-service wilt aansluiten, moet u TLS 1.2 of hoger gebruiken.</span><span class="sxs-lookup"><span data-stu-id="cf11f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="cf11f-107">Probeer de volgende stappen om het TLS-protocol in te schakelen/in te stellen op 1.2, te verifiëren en opnieuw te proberen.</span><span class="sxs-lookup"><span data-stu-id="cf11f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="cf11f-108">Voer bij de opdrachtprompt van\) PowerShell (PS C: voer de volgende opdracht in om het TLS-protocol in te stellen op versie 1.2:</span><span class="sxs-lookup"><span data-stu-id="cf11f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="cf11f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="cf11f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="cf11f-110">Controleer het gebruikte TLS-protocol(en) met de volgende opdracht:</span><span class="sxs-lookup"><span data-stu-id="cf11f-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="cf11f-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="cf11f-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="cf11f-112">Probeer de opdrachten Get of Update indien nodig opnieuw.</span><span class="sxs-lookup"><span data-stu-id="cf11f-112">Retry the Get or Update commands as needed.</span></span>

