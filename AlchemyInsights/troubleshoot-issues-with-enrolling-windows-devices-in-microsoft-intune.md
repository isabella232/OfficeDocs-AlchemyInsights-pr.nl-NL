---
title: Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661518"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="690c1-102">Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven</span><span class="sxs-lookup"><span data-stu-id="690c1-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="690c1-103">Bekijk de bronnen die worden vermeld onder het probleem nu oplossen.</span><span class="sxs-lookup"><span data-stu-id="690c1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="690c1-104">Enkele veelvoorkomende foutberichten en de stappen voor het oplossen:</span><span class="sxs-lookup"><span data-stu-id="690c1-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="690c1-p101">**De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw account-certificaat is verlopen. Het softwarepakket voor de PC-Client in de beheerconsole van Intune opnieuw downloaden. Bekijk deze documentatie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="690c1-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="690c1-108">**Foutcode: 0x801c0003:** De fout kan optreden in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="690c1-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="690c1-p102">De gebruiker heeft meer apparaten dan de apparaatlimiet geregistreerd. Bekijk deze documenten aan [een apparaat verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [wijzigen van de apparaatlimiet](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="690c1-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="690c1-p103">'Gebruikers kunnen deelnemen aan apparaten naar Azure AD' is ingesteld op "none". Stel deze in op alle, of Selecteer gebruikers. Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="690c1-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="690c1-p104">Het apparaat is al door een andere gebruiker ingeschreven. Als dit het geval is, verwijdert u het apparaat uit de console Azure Intune of unenroll handmatig het apparaat voordat u opnieuw probeert.</span><span class="sxs-lookup"><span data-stu-id="690c1-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="690c1-p105">Het apparaat is Windows 10 Home. Alleen Windows 10 Pro, onderwijs en Enterprise SKU's kunt deelnemen aan Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="690c1-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="690c1-118">Aanvullende bronnen voor het oplossen van uw probleem:</span><span class="sxs-lookup"><span data-stu-id="690c1-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="690c1-p106">[Intune probleemoplossing Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken om te bepalen en verhelpen van storingen in gemeenschappelijke inschrijving. Bekijk [Dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="690c1-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="690c1-121">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die voorkomen dat de inschrijving en resoluties aan elk: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) en [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="690c1-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="690c1-122">[Meer informatie over het inschrijven van Windows-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="690c1-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

