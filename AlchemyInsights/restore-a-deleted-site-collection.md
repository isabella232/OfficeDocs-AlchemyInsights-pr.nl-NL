---
title: Een verwijderde site terugzetten
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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552459"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="7b14b-102">Een verwijderde site terugzetten</span><span class="sxs-lookup"><span data-stu-id="7b14b-102">Restore a deleted site</span></span>

<span data-ttu-id="7b14b-103">Wanneer een beheerder een site verwijdert, wordt het geplaatst in de Prullenbak geplaatst, waar het blijft 93 dagen voordat het definitief wordt verwijderd van de siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="7b14b-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="7b14b-104">De site herstellen:</span><span class="sxs-lookup"><span data-stu-id="7b14b-104">To restore the site:</span></span>
  
1. <span data-ttu-id="7b14b-105">In het nieuwe SharePoint admin center, klikt u op **Prullenbak** op het lint.</span><span class="sxs-lookup"><span data-stu-id="7b14b-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7b14b-106">Schakel het selectievakje in naast de siteverzameling die u wilt terugzetten.</span><span class="sxs-lookup"><span data-stu-id="7b14b-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7b14b-107">Klik op **Verwijderde Items herstellen**.</span><span class="sxs-lookup"><span data-stu-id="7b14b-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7b14b-108">Als u een verwijderde communicatiesite herstellen, kunt u de nieuwe SharePoint-admin center.</span><span class="sxs-lookup"><span data-stu-id="7b14b-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="7b14b-109">Anders moet u Microsoft PowerShell gebruiken.</span><span class="sxs-lookup"><span data-stu-id="7b14b-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="7b14b-110">Om terug te zetten op een site die tot een Office 365-groep behoort, moet u de groep in het beheercentrum van Exchange terugzetten.</span><span class="sxs-lookup"><span data-stu-id="7b14b-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="7b14b-111">Groepen kunnen worden hersteld voor 30 dagen nadat ze zijn verwijderd.</span><span class="sxs-lookup"><span data-stu-id="7b14b-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

