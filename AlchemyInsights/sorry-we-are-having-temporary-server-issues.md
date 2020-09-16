---
title: Microsoft 365-apps herstellen er is een bericht over tijdelijke server problemen.
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758240"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="82c0e-102">Het bericht ' er zijn tijdelijke problemen met 365 de server ' wordt opgelost</span><span class="sxs-lookup"><span data-stu-id="82c0e-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="82c0e-103">Als dit bericht wordt weergegeven, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="82c0e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="82c0e-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te controleren of de Internet toegang tot Microsoft 365-apps niet wordt geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="82c0e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="82c0e-105">Zie [url's en IP-](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)adresbereiken.</span><span class="sxs-lookup"><span data-stu-id="82c0e-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="82c0e-106">Ga naar **Start**  >  **Run**en typ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="82c0e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="82c0e-107">Zorg dat de volgende services allemaal worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="82c0e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="82c0e-108">Automatisch instellen met netwerk verbonden apparaten</span><span class="sxs-lookup"><span data-stu-id="82c0e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="82c0e-109">Service voor netwerk lijsten</span><span class="sxs-lookup"><span data-stu-id="82c0e-109">Network List Service</span></span>
    - <span data-ttu-id="82c0e-110">Bewustmaking van netwerklocatie</span><span class="sxs-lookup"><span data-stu-id="82c0e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="82c0e-111">Gebeurtenissenlogboek van Windows</span><span class="sxs-lookup"><span data-stu-id="82c0e-111">Windows Event Log</span></span>

<span data-ttu-id="82c0e-112">Als een van deze services niet actief is, probeert u het programma te starten.</span><span class="sxs-lookup"><span data-stu-id="82c0e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="82c0e-113">Als u problemen ondervindt bij het starten van de service, voert u de volgende opdracht uit als u een opdrachtprompt opent met verhoogde machtigingen:</span><span class="sxs-lookup"><span data-stu-id="82c0e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="82c0e-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="82c0e-114">**sfc /scannow**</span></span>

<span data-ttu-id="82c0e-115">Start de computer opnieuw op nadat u deze opdracht hebt voltooid.</span><span class="sxs-lookup"><span data-stu-id="82c0e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="82c0e-116">Voor meer informatie raadpleegt [u ' Sorry, we kunnen geen verbinding maken met uw account. Probeer het later opnieuw "wanneer u activeert](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="82c0e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>