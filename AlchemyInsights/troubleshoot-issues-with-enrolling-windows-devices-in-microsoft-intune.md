---
title: Problemen oplossen met het registreren van Windows-apparaten in Microsoft intune
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658873"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problemen oplossen met het registreren van Windows-apparaten in Microsoft intune

Bekijk de onderstaande bronnen om uw probleem nu op te lossen.
  
Enkele veelvoorkomende foutberichten en oplossingsstappen:
  
 **De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen. Download het pakket met de PC-client opnieuw in de intune-beheer console. Raadpleeg deze documentatie voor meer informatie.
  
 **Foutcode 0x801c0003:** De fout kan optreden in de volgende scenario's:
  
-  De gebruiker heeft meer apparaten geregistreerd dan de limiet van het apparaat. Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de limiet voor apparaten te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  ' Gebruikers kunnen deelnemen aan een Azure AD ' is ingesteld op ' geen '. Dit instellen op alle of gebruikers selecteren. Raadpleeg [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.

-  Het apparaat is al ingeschreven door een andere gebruiker. Als dat het geval is, verwijdert u het apparaat uit de Azure intune-console of verwijdert u het apparaat handmatig en deregistreren voordat u het opnieuw probeert.

-  Het apparaat is Windows 10 voor thuisgebruik. Alleen Windows 10 Pro, Education en Enterprise Sku's kunnen lid worden van Azure Active Directory.

Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:
  
-  Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving. Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

-  Bekijk deze documenten voor een lijst met veelvoorkomende fouten die kunnen worden ingeschreven en opgelost: voor het [oplossen van problemen](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) en het oplossen van [problemen met doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Meer informatie over het registreren van Windows-apparaten in Microsoft intune](https://docs.microsoft.com/intune/windows-enroll).
