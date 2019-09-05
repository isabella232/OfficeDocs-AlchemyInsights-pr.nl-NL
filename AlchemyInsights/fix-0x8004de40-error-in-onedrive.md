---
title: Fix 0x8004de40 fout in OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755843"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="865ac-102">Fix 0x8004de40 fout in OneDrive</span><span class="sxs-lookup"><span data-stu-id="865ac-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="865ac-103">Als u een fout 0x8004de40 met OneDrive ontvangt:</span><span class="sxs-lookup"><span data-stu-id="865ac-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="865ac-104">Start de betrokken computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.</span><span class="sxs-lookup"><span data-stu-id="865ac-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="865ac-105">Als het probleem niet wordt opgelost door een reboot, loskoppelen en opnieuw deelnemen aan uw apparaat van Azure AD.</span><span class="sxs-lookup"><span data-stu-id="865ac-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="865ac-106">**Opmerking**: u moet zich op uw bedrijfsnetwerk bevinden tijdens het uitvoeren van deze stappen.</span><span class="sxs-lookup"><span data-stu-id="865ac-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="865ac-107">Voer deze stappen niet uit wanneer u geen verbinding maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen).</span><span class="sxs-lookup"><span data-stu-id="865ac-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="865ac-108">Open een opdrachtprompt met verhoogde bevoegdheid.</span><span class="sxs-lookup"><span data-stu-id="865ac-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="865ac-109">Als u wilt een opdrachtprompt met verhoogde bevoegdheid openen, klikt u op-Start, Klik **met**de rechtermuisknop op **opdrachtprompt**en klik vervolgens op **als administrator uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="865ac-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="865ac-110">Typ *dsregcmd/Leave* en druk op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="865ac-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="865ac-111">Als u klaar is, typt u *dsregcmd/join kunnen* en drukt **u op ENTER**.</span><span class="sxs-lookup"><span data-stu-id="865ac-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="865ac-112">Wanneer u klaar is, sluit u de opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="865ac-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="865ac-113">Start de computer opnieuw op en meld u aan bij OneDrive.</span><span class="sxs-lookup"><span data-stu-id="865ac-113">Reboot the computer, and log into OneDrive.</span></span>