---
title: Wi-Fi-profielen van Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555004"
---
# <a name="intune-wi-fi-profiles"></a>Wi-Fi-profielen van Intune

Een succesvolle implementatie van Wi-Fi-connectiviteit voor MDM-clients is afhankelijk van een correct geïmplementeerd profiel dat de vereisten van de zakelijke Wi-Fi-infrastructuur weerspiegelt. Zie voor het bekijken van de juiste instellingen voor de clientplatforms die u onderzoekt: 

[Wi-Fi-instellingen toevoegen voor apparaten met Android in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Wi-Fi-instellingen toevoegen voor speciale en volledig beheerde apparaten van Android Enterprise in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Wi-Fi-instellingen toevoegen voor iOS- en iPadOS-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Wi-Fi-instellingen toevoegen voor Windows 10- en nieuwe apparaten in Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Wi-Fi-instellingen importeren voor Windows-apparaten in Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Veelvoorkomende problemen**

**Ik implementeer een Wi-Fi-profiel dat afhankelijk is van een geïmplementeerd certificaat dat is opgegeven in het Wi-Fi-profiel. De configuratieprofielen vertonen echter een foutstatus.**

Controleer of uw apparaat het certificaat heeft ontvangen.

1. Ga in Intune naar **Alle apparaten** en selecteer het apparaat > **apparaatconfiguratie**.

2. Controleer of alle verwachte profielen worden vermeld en in een succesvolle staat.

3. Als u voor een Android-profiel tussentijdse certificaten in uw certificaatketen hebt, controleert u of ze worden geïmplementeerd op Android-apparaten.

    Als u de certificaatstatus wilt controleren, gaat u naar **Apparaatconfiguratieprofielen**  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.

Als u fouten blijft zien, controleert u de procedures en de secties voor het oplossen van problemen. Zie [Overzicht voor het oplossen van SCEP-certificaatprofielen met Microsoft Intune voor](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)meer informatie.

**Ik heb een Wi-Fi-profiel geïmplementeerd op een apparaat. Intune laat zien dat het succesvol was, maar het apparaat maakt geen verbinding met de Wi-Fi.**

Een succesvolle status betekent dat Intune het profiel heeft geïmplementeerd als geconfigureerd. Deze configuraties komen echter mogelijk niet overeen met uw netwerk- en/of verificatievereisten. Voor meer informatie over de geprobeerde verbinding, controleert u logboeken in de infrastructuur- en verificatieservice (op de Wi-Fi Access Point-controller en NPS/Radius-server). Mogelijk moet u samenwerken met uw netwerkinfrastructuurteam of de wi-fi-leverancier van derden om logboeken te verzamelen en te bekijken.