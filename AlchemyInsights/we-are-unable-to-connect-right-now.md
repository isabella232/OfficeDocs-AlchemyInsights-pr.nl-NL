---
title: Activerings probleem – we kunnen momenteel geen verbinding maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725978"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="02a59-102">Bericht over het herstellen van de Microsoft 365-apps ' we kunnen nu geen verbinding maken '</span><span class="sxs-lookup"><span data-stu-id="02a59-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="02a59-103">Als dit bericht wordt weergegeven, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="02a59-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="02a59-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te controleren of de Internet toegang tot Microsoft 365-apps niet wordt geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="02a59-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="02a59-105">Zie [url's en IP-adresbereiken voor Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="02a59-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="02a59-106">Ga naar **Start**  >  **Run**en typ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="02a59-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="02a59-107">Zorg dat de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="02a59-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="02a59-108">Automatisch instellen met netwerk verbonden apparaten</span><span class="sxs-lookup"><span data-stu-id="02a59-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="02a59-109">Service voor netwerk lijsten</span><span class="sxs-lookup"><span data-stu-id="02a59-109">Network List Service</span></span>
    - <span data-ttu-id="02a59-110">Bewustmaking van netwerklocatie</span><span class="sxs-lookup"><span data-stu-id="02a59-110">Network Location Awareness</span></span>
    - <span data-ttu-id="02a59-111">Gebeurtenissenlogboek van Windows</span><span class="sxs-lookup"><span data-stu-id="02a59-111">Windows Event Log</span></span>

<span data-ttu-id="02a59-112">Als een van deze services niet actief is, probeert u het programma te starten.</span><span class="sxs-lookup"><span data-stu-id="02a59-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="02a59-113">Als u problemen ondervindt bij het starten van de service, voert u de volgende opdracht uit als u een opdrachtprompt opent met verhoogde machtigingen:</span><span class="sxs-lookup"><span data-stu-id="02a59-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="02a59-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="02a59-114">**sfc /scannow**</span></span>

<span data-ttu-id="02a59-115">Start de computer opnieuw op nadat u deze opdracht hebt voltooid.</span><span class="sxs-lookup"><span data-stu-id="02a59-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="02a59-116">Voor meer informatie raadpleegt [u ' Sorry, we kunnen geen verbinding maken met uw account. Probeer het later opnieuw "wanneer u Office activeert bij Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="02a59-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>