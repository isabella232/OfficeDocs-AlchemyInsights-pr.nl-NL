---
title: Activeringsprobleem - We kunnen nu geen verbinding maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716167"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="724f8-102">Het bericht 'We kunnen nu geen verbinding maken' herstellen in de Office-apps</span><span class="sxs-lookup"><span data-stu-id="724f8-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="724f8-103">Als u dit bericht ontvangt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="724f8-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="724f8-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Office-apps niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="724f8-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="724f8-105">Zie [Url's en IP-adresbereiken van Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="724f8-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="724f8-106">Ga naar **Run** > **starten**en typ **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="724f8-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="724f8-107">Controleer of de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="724f8-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="724f8-108">Netwerkverbonden apparaten automatisch instellen</span><span class="sxs-lookup"><span data-stu-id="724f8-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="724f8-109">Netwerklijstservice</span><span class="sxs-lookup"><span data-stu-id="724f8-109">Network List Service</span></span>
    - <span data-ttu-id="724f8-110">Netwerklocatiebewustzijn</span><span class="sxs-lookup"><span data-stu-id="724f8-110">Network Location Awareness</span></span>
    - <span data-ttu-id="724f8-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="724f8-111">Windows Event Log</span></span>

<span data-ttu-id="724f8-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="724f8-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="724f8-113">Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="724f8-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="724f8-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="724f8-114">**sfc /scannow**</span></span>

<span data-ttu-id="724f8-115">Nadat deze opdracht is voltooid, start u de computer opnieuw op.</span><span class="sxs-lookup"><span data-stu-id="724f8-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="724f8-116">Zie ['Sorry, we kunnen geen verbinding maken met uw account' voor meer informatie. Probeer het later opnieuw" fout wanneer u Office activeert vanuit Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="724f8-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>