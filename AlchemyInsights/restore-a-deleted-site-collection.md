---
title: Een verwijderde site terugzetten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692038"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="787ac-102">Een verwijderde site terugzetten</span><span class="sxs-lookup"><span data-stu-id="787ac-102">Restore a deleted site</span></span>

<span data-ttu-id="787ac-103">Wanneer een beheerder een SharePoint-site verwijdert, wordt deze opgeslagen in de Prullenbak van de siteverzameling, die wordt bewaard gedurende 93 dagen voordat deze permanent wordt verwijderd.</span><span class="sxs-lookup"><span data-stu-id="787ac-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="787ac-104">De site terugzetten:</span><span class="sxs-lookup"><span data-stu-id="787ac-104">To restore the site:</span></span>
  
1. <span data-ttu-id="787ac-105">Klik in het nieuwe SharePoint-Beheercentrum op **Prullenbak** op het lint.</span><span class="sxs-lookup"><span data-stu-id="787ac-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="787ac-106">Schakel het selectievakje in naast de siteverzameling die u wilt herstellen.</span><span class="sxs-lookup"><span data-stu-id="787ac-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="787ac-107">Klik op **Verwijderde items herstellen**.</span><span class="sxs-lookup"><span data-stu-id="787ac-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="787ac-108">Als u een verwijderde communicatiesite wilt herstellen, kunt u het nieuwe SharePoint-Beheercentrum gebruiken.</span><span class="sxs-lookup"><span data-stu-id="787ac-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="787ac-109">Anders moet u Microsoft PowerShell gebruiken.</span><span class="sxs-lookup"><span data-stu-id="787ac-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="787ac-110">Als u een site wilt herstellen die deel uitmaakt van een groep Microsoft 365, moet u de groep herstellen in het Exchange-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="787ac-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="787ac-111">Groepen kunnen dertig dagen na verwijdering worden hersteld.</span><span class="sxs-lookup"><span data-stu-id="787ac-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

