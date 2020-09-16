---
title: 0x8004de40 fout in OneDrive oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745125"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="7973a-102">0x8004de40 fout in OneDrive oplossen</span><span class="sxs-lookup"><span data-stu-id="7973a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="7973a-103">Als u een 0x8004de40-fout ontvangt met OneDrive:</span><span class="sxs-lookup"><span data-stu-id="7973a-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="7973a-104">Start de desbetreffende computer opnieuw op terwijl u verbinding hebt met uw Acitve-Directory domein.</span><span class="sxs-lookup"><span data-stu-id="7973a-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="7973a-105">Als het probleem niet is verholpen nadat u de computer opnieuw hebt opgestart, ontkoppelt u uw apparaat en voegt u het opnieuw aan via Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7973a-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="7973a-106">**Opmerking**: u moet zich op uw bedrijfsnetwerk bevinden wanneer u deze stappen uitvoert.</span><span class="sxs-lookup"><span data-stu-id="7973a-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="7973a-107">Voer deze stappen uit als u geen verbinding kunt maken met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens reis).</span><span class="sxs-lookup"><span data-stu-id="7973a-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="7973a-108">Open een opdrachtprompt met verhoogde bevoegdheid.</span><span class="sxs-lookup"><span data-stu-id="7973a-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="7973a-109">Als u een opdrachtprompt met verhoogde bevoegdheid wilt openen, klikt u op **Start**, klikt u met de rechtermuisknop op **opdrachtprompt**en klikt u vervolgens op **als administrator uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="7973a-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="7973a-110">Typ *dsregcmd/Leave* en druk op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7973a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="7973a-111">Wanneer u klaar bent, typt u *dsregcmd/join* en drukt u op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7973a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="7973a-112">Wanneer u klaar bent, sluit u de opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="7973a-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="7973a-113">Start de computer opnieuw op en meld u aan bij OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7973a-113">Reboot the computer, and log into OneDrive.</span></span>