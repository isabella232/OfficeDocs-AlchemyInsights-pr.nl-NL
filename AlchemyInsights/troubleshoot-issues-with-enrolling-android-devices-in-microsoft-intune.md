---
title: Oplossen van problemen met Android apparaten in Microsoft Intune inschrijven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284871"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Oplossen van problemen met Android apparaten in Microsoft Intune inschrijven

Bekijk de bronnen die worden vermeld onder het probleem nu oplossen.
  
Enkele veelvoorkomende problemen en stappen voor het oplossen:
  
 **Apparaat niet fout in de bedrijfsportal gecodeerd:** Nieuwere versies van Android, vooral vanaf v7.0, vereisen een passcode opstarten om te controleren of het apparaat wordt volledig gecodeerd. Algemene oplossingen zijn een pincode opstarten of het apparaat volledig te coderen. Bekijk [Dit document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie. 
  
 **Apparaten niet controleren met de service Intune of als "Unhealthy" weergeven in de beheerconsole van Intune:** Sommige Samsung 4.4 en 5.5 apparaten kunnen niet controleren in de service. Er zijn 3 mogelijke oplossingen voor dit probleem: 
  
1. Open handmatig de bedrijfsportal Intune app, die een apparaat synchroniseren automatisch wordt gestart.
    
2. Werk het apparaat naar Android 6.0 of hoger.
    
3. Samsung Smart Manager uitschakelen in de bedrijfsportal Intune beheren. Bekijk [Dit document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen. 
    
 **Gebruiker licentie Type ongeldige** of **fout gebruiker naam niet herkend:** moet de gebruiker een licentie Intune of EMS worden toegewezen. Bekijk deze documenten een licentie toewijzen: Office Admin Center of Azure portal. 
  
Aanvullende bronnen voor het oplossen van uw probleem:
  
1. [Intune probleemoplossing Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken om te bepalen en verhelpen van storingen in gemeenschappelijke inschrijving. Bekijk [Dit document](https://docs.microsoft.com/en-us/intune/help-desk-operators) voor meer informatie. 
    
2. Bekijk [Dit document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die voorkomen dat de inschrijving en oplossingen voor elk. 
    
3. [Meer informatie over het inschrijven van Android-apparaten in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).
    

