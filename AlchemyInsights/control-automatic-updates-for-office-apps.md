---
title: Automatische updates voor Office Apps beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438993"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="4330b-102">Automatische updates voor Office Apps beheren</span><span class="sxs-lookup"><span data-stu-id="4330b-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="4330b-103">Updates voor Office Apps worden standaard automatisch gedownload en op de achtergrond toegepast zonder tussenkomst van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="4330b-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="4330b-104">Beheerders kunnen echter bepalen hoe updates worden toegepast met behulp van Office Update-instellingen.</span><span class="sxs-lookup"><span data-stu-id="4330b-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="4330b-105">Met de update-instellingen kunnen beheerders automatische updates in- of uitschakelen, de knop **Nu bijwerken** in Office weergeven of verbergen, updatedeadlines instellen en meer.</span><span class="sxs-lookup"><span data-stu-id="4330b-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="4330b-106">Zie voor gedetailleerde informatie:</span><span class="sxs-lookup"><span data-stu-id="4330b-106">For detailed information, see:</span></span>

- [<span data-ttu-id="4330b-107">Update-instellingen voor Office configureren</span><span class="sxs-lookup"><span data-stu-id="4330b-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="4330b-108">Automatisch bijwerken voor Office is niet ingeschakeld</span><span class="sxs-lookup"><span data-stu-id="4330b-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="4330b-109">Definiëren hoe Office wordt bijgewerkt nadat het is geïnstalleerd</span><span class="sxs-lookup"><span data-stu-id="4330b-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="4330b-110">Voer de volgende stappen uit om de bestaande updates-instellingen te controleren die op een clientmachine zijn toegepast:</span><span class="sxs-lookup"><span data-stu-id="4330b-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="4330b-111">Open de registereditor door naar **Start**  >  **Run**  >  **regedit**te gaan.</span><span class="sxs-lookup"><span data-stu-id="4330b-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="4330b-112">Ga naar de volgende locatie en bekijk de instellingen van Office Update:</span><span class="sxs-lookup"><span data-stu-id="4330b-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="4330b-113">a.</span><span class="sxs-lookup"><span data-stu-id="4330b-113">a.</span></span> <span data-ttu-id="4330b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="4330b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="4330b-115">b.</span><span class="sxs-lookup"><span data-stu-id="4330b-115">b.</span></span> <span data-ttu-id="4330b-116">ClickToRun\Configuratie</span><span class="sxs-lookup"><span data-stu-id="4330b-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="4330b-117">**Opmerking**  Als de OfficeMgmtCOM-sleutel is ingesteld, ziet u mogelijk het bericht **Office**'Updates worden beheerd door uw systeembeheerder' in  >  **Office-updates voor**Office office van Office  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="4330b-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="4330b-118">Zie [Updates voor Microsoft 365-apps beheren met Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4330b-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  