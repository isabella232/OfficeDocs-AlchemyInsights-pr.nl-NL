---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708993"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune

Bekijk de onderstaande bronnen om het probleem nu op te lossen.
  
Enkele veelvoorkomende problemen en oplossingen:
  
 **Fout in bedrijfsportal apparaat niet versleuteld:** Voor nieuwere versies van Android, met name die met v7.0, is een opstartcode vereist om ervoor te zorgen dat uw apparaat volledig is versleuteld. Veelvoorkomende oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat. Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.
  
 **Apparaten kunnen niet worden inchecken met de Intune-service** of worden weergegeven als Niet-in orde in de Intune-beheerconsole: Sommige Samsung 4.4- en 5.5-apparaten checken mogelijk niet in bij de service. Er zijn drie mogelijke oplossingen voor dit probleem:
  
1. Open handmatig de Intune-bedrijfsportal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.

2. Werk het apparaat bij naar Android 6.0 of hoger.

3. Schakel Samsung Smart Manager uit voor het beheren van de Intune-bedrijfsportal. Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.

 **Fout: gebruikerslicentietype ongeldig** of gebruikersnaam **niet herkend:** aan de gebruiker moet een Intune- of EMS-licentie worden toegewezen. Bekijk deze documenten om een licentie toe te wijzen via: Office-beheercentrum of Azure Portal.
  
Aanvullende bronnen om het probleem op te lossen:
  
1. Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

2. Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elke fout verhinderen.

3. [Meer informatie over het registreren van Android-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
