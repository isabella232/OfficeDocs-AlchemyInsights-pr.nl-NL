---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689949"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Android-apparaten in Microsoft intune

Bekijk de onderstaande bronnen om uw probleem nu op te lossen.
  
Enkele veelvoorkomende problemen en oplossingsstappen:
  
 **Fout met niet-versleutelde apparaat in de bedrijfs portal:** Voor nieuwere versies van Android, met name vanaf v 7.0, hebt u een opstartwachtwoord code nodig om te controleren of uw apparaat volledig is versleuteld. Veelgebruikte oplossingen zijn om een opstartpincode in te schakelen of het apparaat volledig te versleutelen. Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.
  
 **Apparaten kunnen niet worden ingecheckt met de intune-service of worden niet in de intune-beheerconsole weergegeven:** Bij sommige Samsung 4,4-en 5,5-apparaten werd de service mogelijk niet gecontroleerd. Dit probleem kan drie oplossingen voordoen:
  
1. Open handmatig de app intune Company Portal, waarmee automatisch synchronisatie van apparaten wordt gestart.

2. Werk het apparaat bij naar Android 6,0 of hoger.

3. Schakel Samsung Smart Manager uit voor het beheren van de intune-bedrijfs portal. Bekijk [dit document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.

 Het **gebruikerslicentie type is ongeldig** of de **gebruikersnaam wordt niet herkend:** de gebruiker moet een INtune-of EMS-licentie toewijzen. Bekijk deze documenten om een licentie toe te wijzen via: Office-Beheercentrum of Azure-Portal.
  
Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:
  
1. Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

2. Bekijk [dit document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die niet voor de inschrijving en oplossing zorgen.

3. [Meer informatie over het registreren van Android-apparaten in Microsoft intune](https://docs.microsoft.com/intune/android-enroll).
