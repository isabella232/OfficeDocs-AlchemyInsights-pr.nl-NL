---
title: Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708885"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c068c-102">Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c068c-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c068c-103">Bekijk de onderstaande bronnen om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="c068c-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c068c-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="c068c-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c068c-105">**De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen.</span><span class="sxs-lookup"><span data-stu-id="c068c-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c068c-106">Download het softwarepakket van de PC-client opnieuw in de Intune-beheerconsole.</span><span class="sxs-lookup"><span data-stu-id="c068c-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c068c-107">Bekijk deze documentatie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c068c-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="c068c-108">**Foutcode 0x801c0003:** De fout kan optreden in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="c068c-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="c068c-109">De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet.</span><span class="sxs-lookup"><span data-stu-id="c068c-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c068c-110">Lees deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="c068c-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="c068c-111">'Gebruikers kunnen apparaten deelnemen aan Azure AD' is ingesteld op 'geen'.</span><span class="sxs-lookup"><span data-stu-id="c068c-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="c068c-112">Stel deze in op alle gebruikers of selecteer gebruikers.</span><span class="sxs-lookup"><span data-stu-id="c068c-112">Set it to all or select users.</span></span> <span data-ttu-id="c068c-113">Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c068c-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="c068c-114">Het apparaat is al geregistreerd door een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="c068c-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c068c-115">Als dat het geval is, verwijdert u het apparaat uit de Azure Intune-console of verwijdert u het apparaat handmatig voordat u het opnieuw probeert.</span><span class="sxs-lookup"><span data-stu-id="c068c-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="c068c-116">Het apparaat is Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="c068c-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c068c-117">Alleen Windows 10 Pro-, Education- en Enterprise-SKU's kunnen deelnemen aan Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c068c-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="c068c-118">Aanvullende bronnen om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="c068c-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="c068c-119">Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="c068c-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c068c-120">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c068c-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="c068c-121">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die registratie en oplossingen voor elk van deze fouten [verhinderen:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Handleiding voor probleemoplossing en [probleemoplossing van een document.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="c068c-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="c068c-122">[Meer informatie over het registreren van Windows-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="c068c-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
