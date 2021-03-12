---
title: Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708885"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune

Bekijk de onderstaande bronnen om het probleem nu op te lossen.
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
 **De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen. Download het softwarepakket van de PC-client opnieuw in de Intune-beheerconsole. Bekijk deze documentatie voor meer informatie.
  
 **Foutcode 0x801c0003:** De fout kan optreden in de volgende scenario's:
  
-  De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet. Lees deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  'Gebruikers kunnen apparaten deelnemen aan Azure AD' is ingesteld op 'geen'. Stel deze in op alle gebruikers of selecteer gebruikers. Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.

-  Het apparaat is al geregistreerd door een andere gebruiker. Als dat het geval is, verwijdert u het apparaat uit de Azure Intune-console of verwijdert u het apparaat handmatig voordat u het opnieuw probeert.

-  Het apparaat is Windows 10 Home. Alleen Windows 10 Pro-, Education- en Enterprise-SKU's kunnen deelnemen aan Azure Active Directory.

Aanvullende bronnen om het probleem op te lossen:
  
-  Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

-  Bekijk deze documenten voor een lijst met veelvoorkomende fouten die registratie en oplossingen voor elk van deze fouten [verhinderen:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Handleiding voor probleemoplossing en [probleemoplossing van een document.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Meer informatie over het registreren van Windows-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
