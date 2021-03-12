---
title: Tenantbeleid oplossen (actie overschrijven)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744478"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="35e0e-102">Tenantbeleid oplossen (actie overschrijven)</span><span class="sxs-lookup"><span data-stu-id="35e0e-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="35e0e-103">Dit bericht is beïnvloed door een antispambeleid in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="35e0e-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="35e0e-104">Ga als volgt te werk om het beleid te bekijken:</span><span class="sxs-lookup"><span data-stu-id="35e0e-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="35e0e-105">Ga naar het [Office 365-beveiligings- & compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga vervolgens naar **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="35e0e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="35e0e-106">Controleer of **beleidsbron** het volgende aangeeft:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="35e0e-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="35e0e-107">Als dat zo is, **controleert** u op het tabblad Aangepast de instellingen van het beleid dat van invloed is op het bericht.</span><span class="sxs-lookup"><span data-stu-id="35e0e-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="35e0e-108">Het is mogelijk dat de standaardinstellingen **die** zijn toegepast op alle klanten van Exchange Online Protection, van invloed zijn op het bericht.</span><span class="sxs-lookup"><span data-stu-id="35e0e-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="35e0e-109">Zie Beleidsregels voor spamfilter configureren voor meer informatie over het configureren van beleidsregels voor [spamfilters.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="35e0e-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
