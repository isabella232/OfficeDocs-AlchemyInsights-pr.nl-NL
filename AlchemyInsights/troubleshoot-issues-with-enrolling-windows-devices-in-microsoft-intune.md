---
title: Problemen oplossen met het inschrijven van Windows-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665827"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problemen oplossen met het inschrijven van Windows-apparaten in Microsoft Intune

Bekijk de onderstaande bronnen om het probleem nu op te lossen.
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
 **De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen. Download het pc-clientsoftwarepakket opnieuw in de Intune-beheerconsole. Bekijk deze documentatie voor meer informatie.
  
 **Foutcode 0x801c0003:** De fout kan zich voordoen in de volgende scenario's:
  
-  De gebruiker heeft meer apparaten ingeschreven dan de apparaatlimiet. Controleer deze documenten om [een apparaat](https://docs.microsoft.com/intune/devices-wipe) te verwijderen of [de apparaatlimiet te wijzigen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  'Gebruikers kunnen deelnemen aan apparaten bij Azure AD' is ingesteld op 'geen'. Stel het in op alle of selecteer gebruikers. Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.

-  Het apparaat is al ingeschreven door een andere gebruiker. Als dat het geval is, verwijdert u het apparaat uit de Azure Intune-console of rolt u het apparaat handmatig uit voordat u het opnieuw probeert.

-  Het apparaat is Windows 10 Home. Alleen Windows 10 Pro, Education en Enterprise SKU's kunnen lid worden van Azure Active Directory.

Extra bronnen om uw probleem op te lossen:
  
-  Gebruik [Portal voor het oplossen van problemen bij intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) om veelvoorkomende inschrijvingsfouten te diagnosticeren en op te lossen. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

-  Controleer deze documenten op een lijst met veelvoorkomende fouten die inschrijving en resoluties voor elk voorkomen: [handleiding voor het oplossen van](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) problemen en het oplossen van [problemen.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[Meer informatie over het inschrijven van Windows-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
