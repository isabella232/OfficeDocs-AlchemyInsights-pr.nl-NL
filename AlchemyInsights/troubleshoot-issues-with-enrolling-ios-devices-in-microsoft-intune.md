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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van iOS-apparaten in Microsoft intune

Bekijk de onderstaande bronnen om uw probleem nu op te lossen. 
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
- **Apparaat kapje bereikt** De gebruiker heeft meer apparaten geregistreerd dan de limiet van het apparaat. Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de limiet voor apparaten te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Deze service wordt niet ondersteund. Geen inschrijvingsbeleid:** de Apple Push Notification-Service (APNS) moet zijn geconfigureerd of vernieuwd. Bekijk [dit document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) voor meer informatie over hoe u dat kunt doen. 
    
- **Ongeldig gebruikerslicentie type of gebruikersnaam wordt niet herkend:** De gebruiker moet een intune-of EMS-licentie toewijzen. Bekijk deze documenten om een licentie toe te wijzen via: [Office-Beheercentrum](https://docs.microsoft.com/intune/licenses-assign) of [Azure-Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:
  
1. Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie. 
    
2. Bekijk deze documenten voor een lijst met veelvoorkomende fouten die kunnen worden ingeschreven en opgelost: voor het [oplossen van problemen](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) en het oplossen van [problemen met doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Meer informatie over het registreren van Ios-apparaten in Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).
    

