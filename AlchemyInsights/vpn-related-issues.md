---
title: VPN-gerelateerde problemen
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554971"
---
# <a name="vpn-related-issues"></a>VPN-gerelateerde problemen

Succesvolle implementatie van VPN-connectiviteit voor MDM-clients is afhankelijk van een geïmplementeerd profiel dat de vereisten van de VPN-infrastructuur correct weergeeft. Zie voor de juiste instellingen voor de clientplatforms die u onderzoekt: 

[Windows 10- en Windows-holografische apparaatinstellingen om VPN-verbindingen toe te voegen met Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN-instellingen toevoegen op iOS- en iPadOS-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Instellingen voor Android-apparaten om VPN in Intune te configureren](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN-instellingen toevoegen op macOS-apparaten in Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Als uw VPN-profiel verificatie op basis van certificaten gebruikt, controleert u of de hoofdcertificaat- en clientverificatiecertificaatprofielen die aan het VPN-profiel zijn gekoppeld, met succes worden geïmplementeerd.

**Veelvoorkomende problemen**

**Ik heb een VPN-profiel geïmplementeerd op een apparaat. Intune laat zien dat het succesvol was, maar het apparaat maakt geen verbinding met de VPN.**

Een succesvolle status betekent dat Intune het profiel heeft geïmplementeerd als geconfigureerd. Deze configuraties komen echter mogelijk niet overeen met uw netwerk- en/of verificatievereisten. Bekijk logboeken in de infrastructuur- en verificatieservice (op de VPN-server en NPS/Radius-server) voor meer informatie over de geprobeerde verbinding. Mogelijk moet u samenwerken met uw netwerkinfrastructuurteam of de VPN-leverancier van derden om logboeken te verzamelen en te bekijken.

**Wanneer ik een aangepaste VPN voor iOS configureer, wordt de VPN-functie per app niet beschikbaar gesteld.**

Per-app VPN voor iOS-apparaten in Intune is momenteel beschikbaar voor een specifieke lijst van providers en partners, die ook moeten voldoen aan de certificaatvoorwaarden voordat u een VPN per app configureert. Zie [VPN (Virtual Private Network) instellen per app Virtual Private Network (VPN) instellen voor iOS/iPadOS-apparaten in Intune.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

Zie [VPN-profielen maken om verbinding te maken met VPN-servers in Intune voor](https://docs.microsoft.com/intune/vpn-settings-configure)meer informatie over alle VPN-verbindingstypen in Intune.  

**iOS On-Demand VPN wordt niet geactiveerd wanneer een geconfigureerd domein wordt geopend**

Als u automatische VPN-instellingen wilt testen, stelt u de volgende waarden in:

Ik wil het volgende doen: **Elke verbindingspoging evalueren** 

Kiezen of u verbinding wilt maken: **maak verbinding indien nodig**

Wanneer gebruikers toegang krijgen tot deze domeinen: **target** *doeldomeinnaam*

Als de bovenstaande configuratie niet is geslaagd, voegt u het volgende element toe:

Wanneer deze URL onbereikbaar is, force connect the VPN: **BADURL**