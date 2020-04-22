---
title: Problemen met inschrijvende Android-apparaten in Microsoft Intune oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759615"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problemen met inschrijvende Android-apparaten in Microsoft Intune oplossen

Bekijk de onderstaande bronnen om het probleem nu op te lossen.
  
Enkele veelvoorkomende problemen en stappen voor het oplossen van oplossingen:
  
 **Apparaat niet versleutelde fout in bedrijfsportal:** Nieuwere versies van Android, met name te beginnen met v7.0, vereisen een opstartcode om ervoor te zorgen dat uw apparaat volledig is versleuteld. Veelvoorkomende oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat. Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.
  
 **Apparaten kunnen niet inchecken met de Intune-service of worden weergegeven als 'Niet in orde' in de Intune-beheerconsole:** Sommige Samsung 4.4- en 5.5-apparaten kunnen niet inchecken in de service. Er zijn 3 mogelijke oplossingen voor dit probleem:
  
1. Open handmatig de Intune Company Portal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.

2. Werk het apparaat bij naar Android 6.0 of hoger.

3. Schakel Samsung Smart Manager uit om de Intune Company Portal te beheren. Bekijk [dit document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze kwesties en oplossingen.

 **Ongeldig type gebruikerslicentie** of **gebruikersnaam niet-herkende fout:** de gebruiker moet een Intune- of EMS-licentie toegewezen krijgen. Controleer deze documenten om een licentie toe te wijzen via: Office Admin Center of Azure portal.
  
Aanvullende bronnen om uw probleem op te lossen:
  
1. Gebruik [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) om veelvoorkomende inschrijvingsfouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

2. Controleer [dit document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) op een lijst met veelvoorkomende fouten die inschrijving en resoluties voor elke instelling voorkomen.

3. [Meer informatie over het inschrijven van Android-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
