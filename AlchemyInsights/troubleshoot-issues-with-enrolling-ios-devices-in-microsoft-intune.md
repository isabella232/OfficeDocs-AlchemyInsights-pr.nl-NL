---
title: Problemen met het inschrijven van iOS-apparaten in Microsoft Intune oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736153"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="02f52-102">Problemen met het inschrijven van iOS-apparaten in Microsoft Intune oplossen</span><span class="sxs-lookup"><span data-stu-id="02f52-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="02f52-103">Bekijk de onderstaande bronnen om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="02f52-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="02f52-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="02f52-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="02f52-105">**Apparaatdop bereikt** De gebruiker heeft meer apparaten ingeschreven dan de apparaatlimiet.</span><span class="sxs-lookup"><span data-stu-id="02f52-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="02f52-106">Controleer deze documenten om [een apparaat](https://docs.microsoft.com/intune/devices-wipe) te verwijderen of [de apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="02f52-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="02f52-107">**Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** De Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="02f52-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="02f52-108">Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dat doen.</span><span class="sxs-lookup"><span data-stu-id="02f52-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="02f52-109">**Gebruikerslicentietype ongeldig of gebruikersnaam niet herkend:** De gebruiker moet een Intune- of EMS-licentie toegewezen krijgen.</span><span class="sxs-lookup"><span data-stu-id="02f52-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="02f52-110">Controleer deze documenten om een licentie toe te wijzen via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) of Azure [portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="02f52-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="02f52-111">Aanvullende bronnen om uw probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="02f52-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="02f52-112">Gebruik [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) om veelvoorkomende inschrijvingsfouten te diagnosticeren en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="02f52-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="02f52-113">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="02f52-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="02f52-114">Controleer deze documenten op een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elk: [document voor probleemoplossing](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en [probleemoplossing](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)voorkomen.</span><span class="sxs-lookup"><span data-stu-id="02f52-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="02f52-115">[Meer informatie over het inschrijven van iOS-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="02f52-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

