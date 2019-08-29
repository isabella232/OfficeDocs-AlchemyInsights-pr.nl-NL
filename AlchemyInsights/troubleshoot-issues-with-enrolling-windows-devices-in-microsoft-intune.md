---
title: Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665827"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b07a3-102">Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven</span><span class="sxs-lookup"><span data-stu-id="b07a3-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b07a3-103">Bekijk de bronnen die worden vermeld onder het probleem nu oplossen.</span><span class="sxs-lookup"><span data-stu-id="b07a3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b07a3-104">Enkele veelvoorkomende foutberichten en de stappen voor het oplossen:</span><span class="sxs-lookup"><span data-stu-id="b07a3-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b07a3-105">**De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw account-certificaat is verlopen.</span><span class="sxs-lookup"><span data-stu-id="b07a3-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="b07a3-106">Het softwarepakket voor de PC-Client in de beheerconsole van Intune opnieuw downloaden.</span><span class="sxs-lookup"><span data-stu-id="b07a3-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="b07a3-107">Bekijk deze documentatie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b07a3-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="b07a3-108">**Foutcode: 0x801c0003:** De fout kan optreden in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="b07a3-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="b07a3-109">De gebruiker heeft meer apparaten dan de apparaatlimiet geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="b07a3-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b07a3-110">Bekijk deze documenten aan [een apparaat verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [wijzigen van de apparaatlimiet](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b07a3-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="b07a3-111">'Gebruikers kunnen deelnemen aan apparaten naar Azure AD' is ingesteld op 'geen'.</span><span class="sxs-lookup"><span data-stu-id="b07a3-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="b07a3-112">Stel deze in op alle, of Selecteer gebruikers.</span><span class="sxs-lookup"><span data-stu-id="b07a3-112">Set it to all or select users.</span></span> <span data-ttu-id="b07a3-113">Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b07a3-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="b07a3-114">Het apparaat is al door een andere gebruiker ingeschreven.</span><span class="sxs-lookup"><span data-stu-id="b07a3-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="b07a3-115">Als dit het geval is, verwijdert u het apparaat uit de console Azure Intune of unenroll handmatig het apparaat voordat u opnieuw probeert.</span><span class="sxs-lookup"><span data-stu-id="b07a3-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="b07a3-116">Het apparaat is Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="b07a3-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="b07a3-117">Alleen Windows 10 Pro, onderwijs en Enterprise SKU's kunt deelnemen aan Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b07a3-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="b07a3-118">Aanvullende bronnen voor het oplossen van uw probleem:</span><span class="sxs-lookup"><span data-stu-id="b07a3-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="b07a3-119">[Intune probleemoplossing Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken om te bepalen en verhelpen van storingen in gemeenschappelijke inschrijving.</span><span class="sxs-lookup"><span data-stu-id="b07a3-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b07a3-120">Bekijk [Dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b07a3-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="b07a3-121">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die voorkomen dat de inschrijving en resoluties aan elk: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) en [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b07a3-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="b07a3-122">[Meer informatie over het inschrijven van Windows-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="b07a3-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
