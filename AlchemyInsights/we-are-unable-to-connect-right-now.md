---
title: Activeringsprobleem - We kunnen op dit moment geen verbinding maken
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581870"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="9a6f7-102">Vaststelling van de Microsoft 365 apps "We zijn niet in staat om verbinding te maken op dit moment" bericht</span><span class="sxs-lookup"><span data-stu-id="9a6f7-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="9a6f7-103">Als u dit bericht ontvangt, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="9a6f7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9a6f7-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Microsoft 365-apps niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="9a6f7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9a6f7-105">Zie [Microsoft URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9a6f7-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9a6f7-106">Ga **Start**naar  >  **Start Run**en typ **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="9a6f7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9a6f7-107">Controleer of de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="9a6f7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9a6f7-108">Netwerkgekoppelde apparaten automatisch instellen</span><span class="sxs-lookup"><span data-stu-id="9a6f7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9a6f7-109">Netwerklijstservice</span><span class="sxs-lookup"><span data-stu-id="9a6f7-109">Network List Service</span></span>
    - <span data-ttu-id="9a6f7-110">Netwerklocatiebewustzijn</span><span class="sxs-lookup"><span data-stu-id="9a6f7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9a6f7-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="9a6f7-111">Windows Event Log</span></span>

<span data-ttu-id="9a6f7-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="9a6f7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9a6f7-113">Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="9a6f7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9a6f7-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="9a6f7-114">**sfc /scannow**</span></span>

<span data-ttu-id="9a6f7-115">Nadat deze opdracht is voltooid, start u de computer opnieuw.</span><span class="sxs-lookup"><span data-stu-id="9a6f7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9a6f7-116">Zie ['Sorry, we kunnen geen verbinding maken met je account voor meer informatie. Probeer het later opnieuw" fout wanneer u Office activeert vanuit Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="9a6f7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>