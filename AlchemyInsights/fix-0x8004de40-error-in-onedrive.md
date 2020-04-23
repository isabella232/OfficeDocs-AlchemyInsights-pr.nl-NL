---
title: 0x8004de40-fout oplossen in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716023"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="e4b40-102">0x8004de40-fout oplossen in OneDrive</span><span class="sxs-lookup"><span data-stu-id="e4b40-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="e4b40-103">Als u een fout van 0x8004de40 met OneDrive ontvangt:</span><span class="sxs-lookup"><span data-stu-id="e4b40-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="e4b40-104">Start de betreffende computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.</span><span class="sxs-lookup"><span data-stu-id="e4b40-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="e4b40-105">Als een reboot het probleem niet oplost, sluit u de join en sluit u uw apparaat opnieuw aan vanuit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4b40-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="e4b40-106">**Opmerking:** U moet zich tijdens het uitvoeren van deze stappen in uw bedrijfsnetwerk bevinden.</span><span class="sxs-lookup"><span data-stu-id="e4b40-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="e4b40-107">Voer deze stappen niet uit wanneer u geen verbinding maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen).</span><span class="sxs-lookup"><span data-stu-id="e4b40-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="e4b40-108">Open een opdrachtprompt met verhoogde bevoegdheid.</span><span class="sxs-lookup"><span data-stu-id="e4b40-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="e4b40-109">Als u een opdrachtprompt met verhoogde bevoegdheid wilt openen, klikt u op - **Start**, klikt u met de rechtermuisknop op **Opdrachtprompt**en klikt u vervolgens op **Uitvoeren als beheerder**.</span><span class="sxs-lookup"><span data-stu-id="e4b40-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="e4b40-110">Typ *dsregcmd /leave* en druk op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e4b40-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="e4b40-111">Als u klaar bent, typt u *dsregcmd /join* en drukt u op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e4b40-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="e4b40-112">Als u klaar bent, sluit u de opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="e4b40-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="e4b40-113">Start de computer opnieuw op en meld u aan bij OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e4b40-113">Reboot the computer, and log into OneDrive.</span></span>