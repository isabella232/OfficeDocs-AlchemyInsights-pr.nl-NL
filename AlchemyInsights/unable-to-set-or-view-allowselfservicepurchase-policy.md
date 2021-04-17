---
title: Kan het beleid AllowSelfServicePurchase niet instellen of weergeven
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826086"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9338a-102">Kan het beleid AllowSelfServicePurchase niet instellen of weergeven</span><span class="sxs-lookup"><span data-stu-id="9338a-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9338a-103">Wanneer u het beleid AllowSelfServicePurchase probeert in te stellen of weer te geven, ontvangt u het volgende foutbericht:</span><span class="sxs-lookup"><span data-stu-id="9338a-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9338a-104">*HandleError: Kan het productbeleid niet ophalen met PolicyId 'AllowSelfServicePurchase', ErrorMessage - De onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden bij een verzenden.*</span><span class="sxs-lookup"><span data-stu-id="9338a-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9338a-105">Dit kan het gevolg zijn van een oudere versie van Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="9338a-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9338a-106">Als u verbinding wilt maken met de MSCommerce-service, moet u TLS 1.2 of hoger gebruiken.</span><span class="sxs-lookup"><span data-stu-id="9338a-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9338a-107">Probeer de volgende stappen om het TLS-protocol in te stellen op 1.2, te verifiëren en opnieuw te proberen.</span><span class="sxs-lookup"><span data-stu-id="9338a-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9338a-108">Voer bij de Opdrachtprompt van PowerShell (PS C: voer de volgende opdracht in om het TLS-protocol in te stellen \) op versie 1.2:</span><span class="sxs-lookup"><span data-stu-id="9338a-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="9338a-109">Controleer het TLS-protocol(en) dat in gebruik is, met de volgende opdracht:</span><span class="sxs-lookup"><span data-stu-id="9338a-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="9338a-110">U kunt de opdrachten Downloaden of Bijwerken zo nodig opnieuw proberen.</span><span class="sxs-lookup"><span data-stu-id="9338a-110">Retry the Get or Update commands as needed.</span></span>

