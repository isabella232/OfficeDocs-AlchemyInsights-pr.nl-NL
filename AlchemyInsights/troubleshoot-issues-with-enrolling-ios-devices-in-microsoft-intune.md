---
title: Problemen oplossen met het registreren van iOS-apparaten in Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669243"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="cc173-102">Problemen oplossen met het registreren van iOS-apparaten in Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="cc173-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="cc173-103">Bekijk de onderstaande bronnen om uw probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="cc173-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="cc173-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="cc173-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="cc173-105">**Apparaat kapje bereikt** De gebruiker heeft meer apparaten geregistreerd dan de limiet van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="cc173-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="cc173-106">Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de limiet voor apparaten te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="cc173-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="cc173-107">**Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** de Apple Push Notification-Service (APNS) moet zijn geconfigureerd of vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="cc173-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="cc173-108">Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor meer informatie over hoe u dat kunt doen.</span><span class="sxs-lookup"><span data-stu-id="cc173-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="cc173-109">**Ongeldig gebruikerslicentie type of gebruikersnaam wordt niet herkend:** De gebruiker moet een intune-of EMS-licentie toewijzen.</span><span class="sxs-lookup"><span data-stu-id="cc173-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="cc173-110">Bekijk deze documenten om een licentie toe te wijzen via: [Office-Beheercentrum](https://docs.microsoft.com/intune/licenses-assign) of [Azure-Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="cc173-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="cc173-111">Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:</span><span class="sxs-lookup"><span data-stu-id="cc173-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="cc173-112">Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving.</span><span class="sxs-lookup"><span data-stu-id="cc173-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="cc173-113">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="cc173-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="cc173-114">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die kunnen worden ingeschreven en opgelost: voor het [oplossen van problemen](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en het oplossen van [problemen met doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="cc173-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="cc173-115">[Meer informatie over het registreren van Ios-apparaten in Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="cc173-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

