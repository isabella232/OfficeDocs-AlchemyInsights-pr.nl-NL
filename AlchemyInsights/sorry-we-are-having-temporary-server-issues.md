---
title: Microsoft 365-apps oplossen Sorry, we hebben een bericht over tijdelijke serverproblemen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582698"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="bfe82-102">Het bericht microsoft 365-apps 'Sorry, we hebben tijdelijke serverproblemen' oplossen</span><span class="sxs-lookup"><span data-stu-id="bfe82-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="bfe82-103">Als u dit bericht ontvangt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="bfe82-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bfe82-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Microsoft 365-apps niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="bfe82-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bfe82-105">Zie [URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bfe82-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bfe82-106">Ga **Start**naar  >  **Start Run**en typ **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="bfe82-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bfe82-107">Controleer of de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="bfe82-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bfe82-108">Netwerkgekoppelde apparaten automatisch instellen</span><span class="sxs-lookup"><span data-stu-id="bfe82-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bfe82-109">Netwerklijstservice</span><span class="sxs-lookup"><span data-stu-id="bfe82-109">Network List Service</span></span>
    - <span data-ttu-id="bfe82-110">Netwerklocatiebewustzijn</span><span class="sxs-lookup"><span data-stu-id="bfe82-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bfe82-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="bfe82-111">Windows Event Log</span></span>

<span data-ttu-id="bfe82-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="bfe82-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bfe82-113">Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="bfe82-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bfe82-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="bfe82-114">**sfc /scannow**</span></span>

<span data-ttu-id="bfe82-115">Nadat deze opdracht is voltooid, start u de computer opnieuw.</span><span class="sxs-lookup"><span data-stu-id="bfe82-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bfe82-116">Zie ['Sorry, we kunnen geen verbinding maken met je account voor meer informatie. Probeer het later opnieuw" fout wanneer u activeert](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bfe82-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>