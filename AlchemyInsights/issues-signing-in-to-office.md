---
title: Problemen met het aanmelden bij Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938183"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="9e90c-102">Lege aanmeldingsscherm in Office-toepassingen</span><span class="sxs-lookup"><span data-stu-id="9e90c-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="9e90c-103">U kunt dit probleem oplossen door het volgende proberen:</span><span class="sxs-lookup"><span data-stu-id="9e90c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9e90c-104">Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9e90c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9e90c-105">Opties voor Internet Explorer opnieuw instellen: Ga naar **Extra** > **Internet-opties** > **Geavanceerd** > **Reset Internet Explorer Settings** (Let erop dat u de aangepaste instellingen verliest), en probeer vervolgens het aanmelden bij Office opnieuw.</span><span class="sxs-lookup"><span data-stu-id="9e90c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9e90c-106">Windows Defender-toepassing Guard (WDAG) of een vergelijkbaar programma van de firewall- of antivirusprogramma's uitschakelen:</span><span class="sxs-lookup"><span data-stu-id="9e90c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9e90c-107">Ga naar **Software**in het Configuratiescherm en kies vervolgens **Windows-onderdelen in- of uitschakelen**.</span><span class="sxs-lookup"><span data-stu-id="9e90c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9e90c-108">Als Windows Defender-toepassing beveiliging is ingeschakeld, schakelt u deze.</span><span class="sxs-lookup"><span data-stu-id="9e90c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9e90c-109">**Opmerking:** Wellicht moet u de computer opnieuw opstarten.</span><span class="sxs-lookup"><span data-stu-id="9e90c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9e90c-110">Zorg ervoor dat de Microsoft.AAD.BrokerPlugin [AAD WAM-invoegtoepassing](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) niet wordt geblokkeerd door een toepassing of firewall /-virus.</span><span class="sxs-lookup"><span data-stu-id="9e90c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9e90c-111">[Duidelijke Office referenties](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Referentiebeheer.</span><span class="sxs-lookup"><span data-stu-id="9e90c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9e90c-112">**Opmerking:** De paden voor Office 2016 hebt 16,0 gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="9e90c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9e90c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9e90c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9e90c-114">Voor meer informatie, Zie [problemen met verbinding bij aanmelden nadat deze is bijgewerkt naar Office 2016 build 16.0.7967 op Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9e90c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>