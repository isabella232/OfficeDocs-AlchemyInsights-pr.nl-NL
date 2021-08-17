---
title: Problemen oplossen met het registreren van iOS-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047971"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van iOS-apparaten in Microsoft Intune

Bekijk de onderstaande resources om het probleem nu op te lossen. 
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
- **Apparaatlimiet bereikt** De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet. Bekijk deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Deze service wordt niet ondersteund. Geen registratiebeleid:** Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd. Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dat doet. 
    
- **Gebruikerslicentietype Ongeldig of Gebruikersnaam niet herkend:** Aan de gebruiker moet een Intune- of EMS-licentie worden toegewezen. Bekijk deze documenten om een licentie toe te wijzen via: [Office Beheercentrum](https://docs.microsoft.com/intune/licenses-assign) of [Azure-portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Extra bronnen om het probleem op te lossen:
  
1. Gebruik [Intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie. 
    
2. Bekijk deze documenten voor een lijst met veelvoorkomende fouten die inschrijving verhinderen en voor de oplossing ervan: [Troubleshooting Guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) (Probleemoplossingsgids) en [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) (Probleemoplossingsdocument).
    
3. [Meer informatie over het registreren van iOS-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

