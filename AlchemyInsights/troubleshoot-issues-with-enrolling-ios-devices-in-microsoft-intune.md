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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemen met het inschrijven van iOS-apparaten in Microsoft intune oplossen

Bekijk de hieronder vermelde bronnen om uw probleem nu op te lossen. 
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
- **Apparaatdop bereikt** De gebruiker heeft meer apparaten ingeschreven dan de apparaatlimiet. Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de apparaatlimiet te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** Apple Push Notification Service (APNS) moet worden geconfigureerd of vernieuwd. Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor instructies over hoe u dat moet doen. 
    
- **Gebruikerslicentie type ongeldig of gebruikersnaam niet herkend:** Aan de gebruiker moet een intune-of EMS-licentie worden toegewezen. Bekijk deze documenten om een licentie toe te wijzen via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) of [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Aanvullende hulpmiddelen om uw probleem op te lossen:
  
1. [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken voor het opsporen en oplossen van veelvoorkomende inschrijvings fouten. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie. 
    
2. Bekijk deze documenten voor een lijst met veelvoorkomende fouten die voorkomen dat inschrijving en oplossingen voor elk: [Troubleshooting gids](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Meer informatie over het inschrijven van Ios-apparaten in Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).
    

