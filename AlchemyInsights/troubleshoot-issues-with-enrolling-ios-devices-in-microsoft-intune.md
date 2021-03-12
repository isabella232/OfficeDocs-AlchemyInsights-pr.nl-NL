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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van iOS-apparaten in Microsoft Intune

Bekijk de onderstaande bronnen om het probleem nu op te lossen. 
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
- **Apparaatlimiet bereikt** De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet. Lees deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Deze Service wordt niet ondersteund. Geen registratiebeleid:** Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd. Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dit kunt doen. 
    
- **Gebruikerslicentietype Ongeldig of Gebruikersnaam niet herkend:** Aan de gebruiker moet een Intune- of EMS-licentie worden toegewezen. Bekijk deze documenten om een licentie toe te wijzen via: [Office-beheercentrum](https://docs.microsoft.com/intune/licenses-assign) of [Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Aanvullende bronnen om het probleem op te lossen:
  
1. Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie. 
    
2. Bekijk deze documenten voor een lijst met veelvoorkomende fouten die registratie en oplossingen voor elk van deze fouten [verhinderen:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Handleiding voor probleemoplossing en [probleemoplossing van een document.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Meer informatie over het registreren van iOS-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

