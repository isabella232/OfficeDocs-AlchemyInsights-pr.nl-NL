---
title: Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353532"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Oplossen van problemen met Windows-apparaten in Microsoft Intune inschrijven

Bekijk de bronnen die worden vermeld onder het probleem nu oplossen.
  
Enkele veelvoorkomende foutberichten en de stappen voor het oplossen:
  
 **De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw account-certificaat is verlopen. Het softwarepakket voor de PC-Client in de beheerconsole van Intune opnieuw downloaden. Bekijk deze documentatie voor meer informatie.
  
 **Foutcode: 0x801c0003:** De fout kan optreden in de volgende scenario's:
  
1. De gebruiker heeft meer apparaten dan de apparaatlimiet geregistreerd. Bekijk deze documenten aan [een apparaat verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [wijzigen van de apparaatlimiet](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. 'Gebruikers kunnen deelnemen aan apparaten naar Azure AD' is ingesteld op "none". Stel deze in op alle, of Selecteer gebruikers. Bekijk [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.

3. Het apparaat is al door een andere gebruiker ingeschreven. Als dit het geval is, verwijdert u het apparaat uit de console Azure Intune of unenroll handmatig het apparaat voordat u opnieuw probeert.

4. Het apparaat is Windows 10 Home. Alleen Windows 10 Pro, onderwijs en Enterprise SKU's kunt deelnemen aan Azure Active Directory.

Aanvullende bronnen voor het oplossen van uw probleem:
  
1. [Intune probleemoplossing Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) gebruiken om te bepalen en verhelpen van storingen in gemeenschappelijke inschrijving. Bekijk [Dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.

2. Bekijk deze documenten voor een lijst met veelvoorkomende fouten die voorkomen dat de inschrijving en resoluties aan elk: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) en [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Meer informatie over het inschrijven van Windows-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
