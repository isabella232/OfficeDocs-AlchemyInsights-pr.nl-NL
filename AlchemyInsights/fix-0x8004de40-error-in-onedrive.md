---
title: 0x8004de40-fout oplossen in OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525054"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="41c84-102">0x8004de40-fout oplossen in OneDrive</span><span class="sxs-lookup"><span data-stu-id="41c84-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="41c84-103">Als er een fout 0x8004de40 met OneDrive:</span><span class="sxs-lookup"><span data-stu-id="41c84-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="41c84-104">Start opnieuw op de desbetreffende computer terwijl verbonden met uw Acitve Directory-domein.</span><span class="sxs-lookup"><span data-stu-id="41c84-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="41c84-105">Als opnieuw opstarten het probleem niet is verholpen, loskoppelen en weer lid worden van het apparaat uit Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="41c84-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="41c84-106">**Opmerking**: U moet op uw bedrijfsnetwerk worden tijdens het uitvoeren van deze stappen.</span><span class="sxs-lookup"><span data-stu-id="41c84-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="41c84-107">Niet deze stappen niet uitvoeren wanneer u geen verbinding kunnen maken met uw bedrijfsinfrastructuur (bijvoorbeeld wanneer u onderweg bent).</span><span class="sxs-lookup"><span data-stu-id="41c84-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="41c84-108">Open een opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="41c84-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="41c84-109">U opent een opdrachtprompt, op - **Start**, klik met de rechtermuisknop op **opdrachtprompt**en klik vervolgens op **Als administrator uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="41c84-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="41c84-110">*Dsregcmd /leave* en druk op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="41c84-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="41c84-111">Als alles klaar is, *dsregcmd, /join* en druk op **Enter**.</span><span class="sxs-lookup"><span data-stu-id="41c84-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="41c84-112">Als alles klaar is, sluit u de opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="41c84-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="41c84-113">Start de computer opnieuw op en meld u aan bij OneDrive.</span><span class="sxs-lookup"><span data-stu-id="41c84-113">Reboot the computer, and log into OneDrive.</span></span>