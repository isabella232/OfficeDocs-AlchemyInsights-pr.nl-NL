---
title: Activeringsprobleem-we kunnen nu geen verbinding maken
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628237"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="a664b-102">De Office-apps repareren "we kunnen nu geen verbinding maken" bericht</span><span class="sxs-lookup"><span data-stu-id="a664b-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="a664b-103">Als dit bericht wordt weergegeven, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="a664b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a664b-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze Internet toegang tot Office-apps niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="a664b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="a664b-105">Zie [Office 365-url's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a664b-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a664b-106">Ga naar **Start** > **uitvoeren**, en typ vervolgens **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="a664b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a664b-107">Zorg ervoor dat de volgende services worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="a664b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a664b-108">Netwerk verbonden apparaten Auto-Setup</span><span class="sxs-lookup"><span data-stu-id="a664b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a664b-109">Network List service</span><span class="sxs-lookup"><span data-stu-id="a664b-109">Network List Service</span></span>
    - <span data-ttu-id="a664b-110">Netwerklocatie bewustzijn</span><span class="sxs-lookup"><span data-stu-id="a664b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a664b-111">Windows-gebeurtenislogboek</span><span class="sxs-lookup"><span data-stu-id="a664b-111">Windows Event Log</span></span>

<span data-ttu-id="a664b-112">Als een van deze services niet wordt uitgevoerd, probeert u deze te starten.</span><span class="sxs-lookup"><span data-stu-id="a664b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a664b-113">Als u een probleem ondervindt bij het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:</span><span class="sxs-lookup"><span data-stu-id="a664b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a664b-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="a664b-114">**sfc /scannow**</span></span>

<span data-ttu-id="a664b-115">Start de computer opnieuw op nadat deze opdracht is voltooid.</span><span class="sxs-lookup"><span data-stu-id="a664b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a664b-116">Zie [' Sorry, we kunnen geen verbinding maken met uw account ' voor gedetailleerde informatie. Probeer het later opnieuw ' fout bij het activeren van Office van Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a664b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>