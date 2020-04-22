---
title: Office-apps oplossen Helaas hebben we een bericht over tijdelijke serverproblemen
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764112"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="608ed-102">Het bericht 'Sorry, we hebben tijdelijke serverproblemen'</span><span class="sxs-lookup"><span data-stu-id="608ed-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="608ed-103">Als u dit bericht ontvangt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="608ed-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="608ed-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Office-apps niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="608ed-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="608ed-105">Zie [URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="608ed-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="608ed-106">Ga naar **Run** > **starten**en typ **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="608ed-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="608ed-107">Controleer of de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="608ed-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="608ed-108">Netwerkverbonden apparaten automatisch instellen</span><span class="sxs-lookup"><span data-stu-id="608ed-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="608ed-109">Netwerklijstservice</span><span class="sxs-lookup"><span data-stu-id="608ed-109">Network List Service</span></span>
    - <span data-ttu-id="608ed-110">Netwerklocatiebewustzijn</span><span class="sxs-lookup"><span data-stu-id="608ed-110">Network Location Awareness</span></span>
    - <span data-ttu-id="608ed-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="608ed-111">Windows Event Log</span></span>

<span data-ttu-id="608ed-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="608ed-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="608ed-113">Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="608ed-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="608ed-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="608ed-114">**sfc /scannow**</span></span>

<span data-ttu-id="608ed-115">Nadat deze opdracht is voltooid, start u de computer opnieuw op.</span><span class="sxs-lookup"><span data-stu-id="608ed-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="608ed-116">Zie ['Sorry, we kunnen geen verbinding maken met uw account' voor meer informatie. Probeer het later opnieuw" fout wanneer u activeert](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="608ed-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>