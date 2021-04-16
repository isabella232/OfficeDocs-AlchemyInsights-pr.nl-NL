---
title: Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808966"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Windows-apparaten in Microsoft Intune

Bekijk de onderstaande resources om het probleem nu op te lossen.
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
 **De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen. Download het softwarepakket van de pc-client opnieuw in de Intune-beheerconsole. Bekijk deze documentatie voor meer informatie.
  
 **Foutcode 0x801c0003:** De fout kan optreden in de volgende scenario's:
  
-  De gebruiker heeft meer apparaten geregistreerd dan de apparaatlimiet. Bekijk deze documenten om [een apparaat te verwijderen of](https://docs.microsoft.com/intune/devices-wipe) de [apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  'Gebruikers kunnen apparaten deelnemen aan Azure AD' is ingesteld op 'geen'. Stel dit in op alle gebruikers of selecteer gebruikers. Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.

-  Het apparaat is al geregistreerd door een andere gebruiker. Als dat het geval is, verwijdert u het apparaat uit de Azure Intune-console of verwijdert u het apparaat handmatig voordat u het opnieuw probeert.

-  Het apparaat is Windows 10 Home. Alleen SKU's voor Windows 10 Pro, Education en Enterprise kunnen deelnemen aan Azure Active Directory.

Extra bronnen om het probleem op te lossen:
  
-  Gebruik [Intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

-  Bekijk deze documenten voor een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elk document voorkomen: [Handleiding](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) voor probleemoplossing en [Document probleemoplossing.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Meer informatie over het registreren van Windows-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
