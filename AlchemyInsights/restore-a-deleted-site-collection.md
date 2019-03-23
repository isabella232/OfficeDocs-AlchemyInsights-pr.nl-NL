---
title: Een verwijderde siteverzameling herstellen
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753781"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="8afc1-102">Een verwijderde siteverzameling herstellen</span><span class="sxs-lookup"><span data-stu-id="8afc1-102">Restore a deleted site collection</span></span>

<span data-ttu-id="8afc1-103">Wanneer een beheerder een klassieke siteverzameling verwijdert, wordt het geplaatst in de Prullenbak geplaatst, waar het blijft 93 dagen voordat het definitief wordt verwijderd van de siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="8afc1-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="8afc1-104">De siteverzameling herstellen:</span><span class="sxs-lookup"><span data-stu-id="8afc1-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="8afc1-105">In het klassieke SharePoint admin center, klikt u op **Prullenbak** op het lint.</span><span class="sxs-lookup"><span data-stu-id="8afc1-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="8afc1-106">Schakel het selectievakje in naast de siteverzameling die u wilt terugzetten.</span><span class="sxs-lookup"><span data-stu-id="8afc1-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="8afc1-107">Klik op **Verwijderde Items herstellen**.</span><span class="sxs-lookup"><span data-stu-id="8afc1-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="8afc1-108">Als u een verwijderde communicatiesite herstellen, kunt u de nieuwe SharePoint-admin center voorvertoning.</span><span class="sxs-lookup"><span data-stu-id="8afc1-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="8afc1-109">Anders moet u PowerShell gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8afc1-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="8afc1-110">Om terug te zetten op een site die tot een Office 365-groep behoort, moet u de groep in het beheercentrum van Exchange terugzetten.</span><span class="sxs-lookup"><span data-stu-id="8afc1-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="8afc1-111">Groepen kunnen worden hersteld voor 30 dagen nadat ze zijn verwijderd.</span><span class="sxs-lookup"><span data-stu-id="8afc1-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

