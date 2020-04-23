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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemen met het inschrijven van iOS-apparaten in Microsoft Intune oplossen

Bekijk de onderstaande bronnen om het probleem nu op te lossen. 
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
- **Apparaatdop bereikt** De gebruiker heeft meer apparaten ingeschreven dan de apparaatlimiet. Controleer deze documenten om [een apparaat](https://docs.microsoft.com/intune/devices-wipe) te verwijderen of [de apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** De Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd. Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dat doen. 
    
- **Gebruikerslicentietype ongeldig of gebruikersnaam niet herkend:** De gebruiker moet een Intune- of EMS-licentie toegewezen krijgen. Controleer deze documenten om een licentie toe te wijzen via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) of Azure [portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Aanvullende bronnen om uw probleem op te lossen:
  
1. Gebruik [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) om veelvoorkomende inschrijvingsfouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie. 
    
2. Controleer deze documenten op een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elk: [document voor probleemoplossing](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en [probleemoplossing](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)voorkomen.
    
3. [Meer informatie over het inschrijven van iOS-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

