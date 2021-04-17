---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830937"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune

Bekijk de onderstaande resources om het probleem nu op te lossen.
  
Enkele veelvoorkomende problemen en oplossingsstappen:
  
 **Fout apparaat niet versleuteld in bedrijfsportal:** Voor nieuwere versies van Android, met name vanaf v7.0, is een wachtwoordcode voor opstarten vereist om ervoor te zorgen dat uw apparaat volledig is versleuteld. Veelgebruikte oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat. Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.
  
 **Apparaten kunnen niet inchecken met de Intune-service of weergeven als 'Ongezond' in de Intune-beheerconsole:** Sommige Samsung 4.4- en 5.5-apparaten kunnen mogelijk niet inchecken bij de service. Er zijn drie mogelijke oplossingen voor dit probleem:
  
1. Open handmatig de Intune Company Portal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.

2. Werk het apparaat bij naar Android 6.0 of hoger.

3. Schakel Samsung Smart Manager uit om de Intune Company Portal te beheren. Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.

 **Fout bij gebruikerslicentietype Ongeldig** of Niet-herkende **gebruikersnaam:** De gebruiker moet een Intune- of EMS-licentie krijgen. Controleer deze documenten om een licentie toe te wijzen via: Office-beheercentrum of Azure-portal.
  
Extra bronnen om het probleem op te lossen:
  
1. Gebruik [Intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

2. Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elk document voorkomen.

3. [Meer informatie over het registreren van Android-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
