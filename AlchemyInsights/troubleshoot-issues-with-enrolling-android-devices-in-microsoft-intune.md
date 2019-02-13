---
title: Oplossen van problemen met Android apparaten in Microsoft Intune inschrijven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939343"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ce58f-102">Oplossen van problemen met Android apparaten in Microsoft Intune inschrijven</span><span class="sxs-lookup"><span data-stu-id="ce58f-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ce58f-103">Bekijk de bronnen die worden vermeld onder het probleem nu oplossen.</span><span class="sxs-lookup"><span data-stu-id="ce58f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ce58f-104">Enkele veelvoorkomende problemen en stappen voor het oplossen:</span><span class="sxs-lookup"><span data-stu-id="ce58f-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ce58f-p101">**Apparaat niet fout in de bedrijfsportal gecodeerd:** Nieuwere versies van Android, vooral vanaf v7.0, vereisen een passcode opstarten om te controleren of het apparaat wordt volledig gecodeerd. Algemene oplossingen zijn een pincode opstarten of het apparaat volledig te coderen. Bekijk [Dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ce58f-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="ce58f-p102">**Apparaten niet controleren met de service Intune of als "Unhealthy" weergeven in de beheerconsole van Intune:** Sommige Samsung 4.4 en 5.5 apparaten kunnen niet controleren in de service. Er zijn 3 mogelijke oplossingen voor dit probleem:</span><span class="sxs-lookup"><span data-stu-id="ce58f-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="ce58f-110">Open handmatig de bedrijfsportal Intune app, die een apparaat synchroniseren automatisch wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="ce58f-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="ce58f-111">Werk het apparaat naar Android 6.0 of hoger.</span><span class="sxs-lookup"><span data-stu-id="ce58f-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="ce58f-p103">Samsung Smart Manager uitschakelen in de bedrijfsportal Intune beheren. Bekijk [Dit document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="ce58f-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="ce58f-p104">**Gebruiker licentie Type ongeldige** of **fout gebruiker naam niet herkend:** moet de gebruiker een licentie Intune of EMS worden toegewezen. Bekijk deze documenten een licentie toewijzen: Office Admin Center of Azure portal.</span><span class="sxs-lookup"><span data-stu-id="ce58f-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="ce58f-116">Aanvullende bronnen voor het oplossen van uw probleem:</span><span class="sxs-lookup"><span data-stu-id="ce58f-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ce58f-p105">[Intune probleemoplossing Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken om te bepalen en verhelpen van storingen in gemeenschappelijke inschrijving. Bekijk [Dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ce58f-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ce58f-119">Bekijk [Dit document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die voorkomen dat de inschrijving en oplossingen voor elk.</span><span class="sxs-lookup"><span data-stu-id="ce58f-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="ce58f-120">[Meer informatie over het inschrijven van Android-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ce58f-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

