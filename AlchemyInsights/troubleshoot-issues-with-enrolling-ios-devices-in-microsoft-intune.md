---
title: Problemen met het inschrijven van iOS-apparaten in Microsoft intune oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506918"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="51e67-102">Problemen met het inschrijven van iOS-apparaten in Microsoft intune oplossen</span><span class="sxs-lookup"><span data-stu-id="51e67-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="51e67-103">Bekijk de hieronder vermelde bronnen om uw probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="51e67-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="51e67-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="51e67-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="51e67-105">**Apparaatdop bereikt** De gebruiker heeft meer apparaten ingeschreven dan de apparaatlimiet.</span><span class="sxs-lookup"><span data-stu-id="51e67-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="51e67-106">Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de apparaatlimiet te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="51e67-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="51e67-107">**Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="51e67-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="51e67-108">Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dat moet doen.</span><span class="sxs-lookup"><span data-stu-id="51e67-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="51e67-109">**Gebruikerslicentie type ongeldig of gebruikersnaam niet herkend:** Aan de gebruiker moet een intune-of EMS-licentie worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="51e67-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="51e67-110">Bekijk deze documenten om een licentie toe te wijzen via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) of [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="51e67-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="51e67-111">Aanvullende hulpmiddelen om uw probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="51e67-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="51e67-112">[Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken voor het opsporen en oplossen van veelvoorkomende inschrijvings fouten.</span><span class="sxs-lookup"><span data-stu-id="51e67-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="51e67-113">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="51e67-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="51e67-114">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die voorkomen dat inschrijving en oplossingen voor elk: [Troubleshooting gids](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="51e67-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="51e67-115">[Meer informatie over het inschrijven van Ios-apparaten in Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="51e67-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

