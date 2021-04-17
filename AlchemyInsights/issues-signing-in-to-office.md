---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833026"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="0a310-102">Leeg aanmeldingsscherm in Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="0a310-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="0a310-103">Probeer het volgende om dit probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="0a310-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="0a310-104">Installeer de meest recente updates [voor Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="0a310-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0a310-105">Opties voor Internet Explorer opnieuw instellen: Ga naar **Hulpprogramma's**  >  **Internetopties** Geavanceerd  >    >  **Internet Explorer-instellingen** opnieuw instellen (houd er rekening mee dat aangepaste instellingen verloren gaan) en probeer u opnieuw aan te melden bij Office.</span><span class="sxs-lookup"><span data-stu-id="0a310-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="0a310-106">Schakel de Windows Defender Application Guard (WDAG) of een soortgelijk firewall- of antivirusprogramma uit:</span><span class="sxs-lookup"><span data-stu-id="0a310-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="0a310-107">Ga in het Configuratiescherm naar **Programma's** en kies **Vervolgens Windows-functies in- of uitschakelen.**</span><span class="sxs-lookup"><span data-stu-id="0a310-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="0a310-108">Als Windows Defender Application Guard is ingeschakeld, kunt u deze uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="0a310-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="0a310-109">**Opmerking:** Mogelijk moet u de computer opnieuw opstarten.</span><span class="sxs-lookup"><span data-stu-id="0a310-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="0a310-110">Zorg ervoor dat de Microsoft.AAD.MakelaarPlugin [AAD WAM-insteektoepassing](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) niet wordt geblokkeerd door een toepassing of firewall/anti-virusprogramma.</span><span class="sxs-lookup"><span data-stu-id="0a310-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="0a310-111">[Office-referenties met](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.</span><span class="sxs-lookup"><span data-stu-id="0a310-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0a310-112">**Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="0a310-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0a310-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0a310-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="0a310-114">Zie Verbindingsproblemen in aanmelding na update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0a310-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>