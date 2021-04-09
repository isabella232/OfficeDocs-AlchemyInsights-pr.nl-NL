---
title: Fout 0x8004de40 in OneDrive oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649743"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f5cce-102">Fout 0x8004de40 in OneDrive oplossen</span><span class="sxs-lookup"><span data-stu-id="f5cce-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f5cce-103">Als u Windows 7 gebruikt en deze fout ontvangt, kunt u bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)in te stellen als standaardveilige protocollen in WinHTTP in Windows.</span><span class="sxs-lookup"><span data-stu-id="f5cce-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="f5cce-104">Als u Windows 10 gebruikt en u een foutmelding 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="f5cce-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f5cce-105">Start de betreffende computer opnieuw op terwijl deze is verbonden met uw Acitve Directory-domein.</span><span class="sxs-lookup"><span data-stu-id="f5cce-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f5cce-106">Als het probleem niet wordt opgelost door opnieuw op te starten, ontvoegt u het apparaat en maakt u opnieuw gebruik van Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f5cce-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f5cce-107">**Opmerking:** u moet in uw bedrijfsnetwerk zijn terwijl u deze stappen voert.</span><span class="sxs-lookup"><span data-stu-id="f5cce-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f5cce-108">Voer deze stappen niet uit wanneer u niet bent verbonden met uw bedrijfsinfrastructuur (bijvoorbeeld tijdens het reizen).</span><span class="sxs-lookup"><span data-stu-id="f5cce-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="f5cce-109">Open een opdrachtprompt met verhoogde opdracht door **Start** te selecteren, met de rechtermuisknop op **Opdrachtprompt** te klikken en vervolgens **Uitvoeren als beheerder te selecteren.**</span><span class="sxs-lookup"><span data-stu-id="f5cce-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="f5cce-110">Typ *dsregcmd /leave* en druk op **Enter.**</span><span class="sxs-lookup"><span data-stu-id="f5cce-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="f5cce-111">Als u klaar is, *typt u dsregcmd /join en drukt* u op **Enter.**</span><span class="sxs-lookup"><span data-stu-id="f5cce-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="f5cce-112">Als u klaar is, sluit u de opdrachtprompt.</span><span class="sxs-lookup"><span data-stu-id="f5cce-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="f5cce-113">Start de computer opnieuw op en meld u aan bij OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f5cce-113">Reboot the computer, and log into OneDrive.</span></span>