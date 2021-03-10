---
title: Tenantbeleid herstellen (actie overschrijven)
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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693256"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="ad1ab-102">Tenantbeleid herstellen (actie overschrijven)</span><span class="sxs-lookup"><span data-stu-id="ad1ab-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="ad1ab-103">Dit bericht is beïnvloed door een antispambeleid in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="ad1ab-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="ad1ab-104">Ga als volgt te werk om het beleid te controleren:</span><span class="sxs-lookup"><span data-stu-id="ad1ab-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="ad1ab-105">Ga naar het [Office 365-& compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga naar Het beleid voor bedreigingsbeheer  >    >  [antispam.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="ad1ab-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="ad1ab-106">Controleer of de **beleidsbron** het volgende aangeeft:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="ad1ab-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="ad1ab-107">Als dit het zo is, controleert u op **het** tabblad Aangepast de instellingen van het beleid dat van invloed is op het bericht.</span><span class="sxs-lookup"><span data-stu-id="ad1ab-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="ad1ab-108">Mogelijk zijn de **standaardinstellingen** van toepassing op alle klanten van Exchange Online Protection die van invloed zijn op het bericht.</span><span class="sxs-lookup"><span data-stu-id="ad1ab-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="ad1ab-109">Zie Het spamfilterbeleid configureren voor meer informatie over het configureren van [spamfilterbeleid.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="ad1ab-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
