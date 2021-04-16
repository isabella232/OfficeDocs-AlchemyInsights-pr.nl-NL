---
title: 'Activeringsprobleem: we kunnen momenteel geen verbinding maken'
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806437"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b1ef9-102">Fix the Microsoft 365 apps "We are unable to connect right now" bericht</span><span class="sxs-lookup"><span data-stu-id="b1ef9-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b1ef9-103">Als u dit bericht ontvangt, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="b1ef9-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b1ef9-104">Controleer uw firewall-, antivirussoftware- en proxy-instellingen om te bevestigen dat ze geen internetverbinding blokkeren voor Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="b1ef9-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b1ef9-105">Zie [Microsoft URL's en IP-adresbereiken.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b1ef9-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b1ef9-106">Ga naar **Start**  >  **Run** en typ **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="b1ef9-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b1ef9-107">Zorg ervoor dat de volgende services worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="b1ef9-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b1ef9-108">Auto-setup van verbonden netwerkapparaten</span><span class="sxs-lookup"><span data-stu-id="b1ef9-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b1ef9-109">Netwerklijstservice</span><span class="sxs-lookup"><span data-stu-id="b1ef9-109">Network List Service</span></span>
    - <span data-ttu-id="b1ef9-110">Netwerklocatiebekendheid</span><span class="sxs-lookup"><span data-stu-id="b1ef9-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b1ef9-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="b1ef9-111">Windows Event Log</span></span>

<span data-ttu-id="b1ef9-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="b1ef9-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b1ef9-113">Als u een probleem hebt met het starten van de service, kunt u de volgende opdracht uitvoeren door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="b1ef9-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b1ef9-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="b1ef9-114">**sfc /scannow**</span></span>

<span data-ttu-id="b1ef9-115">Nadat deze opdracht is klaar, start u de computer opnieuw op.</span><span class="sxs-lookup"><span data-stu-id="b1ef9-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b1ef9-116">Zie 'Sorry, we kunnen geen verbinding maken met uw account' voor [meer informatie. Probeer het later opnieuw' fout wanneer u Office activeert vanuit Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="b1ef9-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>