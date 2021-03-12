---
title: Problemen oplossen met het registreren van iOS-apparaten in Microsoft Intune
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708957"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b442b-102">Problemen oplossen met het registreren van iOS-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b442b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b442b-103">Bekijk de onderstaande bronnen om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="b442b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b442b-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="b442b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b442b-105">**Apparaatlimiet bereikt** De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet.</span><span class="sxs-lookup"><span data-stu-id="b442b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b442b-106">Lees deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="b442b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b442b-107">**Deze Service wordt niet ondersteund. Geen registratiebeleid:** Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="b442b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="b442b-108">Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dit kunt doen.</span><span class="sxs-lookup"><span data-stu-id="b442b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b442b-109">**Gebruikerslicentietype Ongeldig of Gebruikersnaam niet herkend:** Aan de gebruiker moet een Intune- of EMS-licentie worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="b442b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b442b-110">Bekijk deze documenten om een licentie toe te wijzen via: [Office-beheercentrum](https://docs.microsoft.com/intune/licenses-assign) of [Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="b442b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b442b-111">Aanvullende bronnen om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="b442b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b442b-112">Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="b442b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b442b-113">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b442b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b442b-114">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die registratie en oplossingen voor elk van deze fouten [verhinderen:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Handleiding voor probleemoplossing en [probleemoplossing van een document.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b442b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b442b-115">[Meer informatie over het registreren van iOS-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="b442b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

