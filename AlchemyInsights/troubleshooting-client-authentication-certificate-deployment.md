---
title: Implementatie van clientverificatiecertificaten oplossen
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555003"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Implementatie van clientverificatiecertificaten oplossen

Intune NDES/SCEP en PKCS/PFX Client certificaten profielen profielen worden vaak gebruikt in combinatie met andere profielen types zoals Wifi, VPN, en e-mail om gebruikers te authenticeren om corporate resources. Wanneer deze profieltypen zijn gekoppeld aan een clientcertificaatprofiel, zijn ze afhankelijk van de succesvolle implementatie van dat profiel.

De eerste infrastructuurinstelling en de bijbehorende configuratie van het clientcertificaatprofiel vereisen vaak probleemoplossing. Zie voor een stapsgewijze handleiding voor het succesvol instellen van de NDES-connector en richtlijnen voor het oplossen van problemen met de implementatie van certificaten: 

- [Infrastructuur configureren om SCEP te ondersteunen met Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Overzicht voor het oplossen van SCEP-certificaatprofielen met Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Gebruik de powershell-scripts waarnaar wordt verwezen om uw configuratie te verifiëren. Zie [Verificatiescripts voor Intune Certificate-connector voor](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)meer informatie .

  
**Andere veelvoorkomende kwesties**

**Wanneer ik de Intune-certificaatconnector op de NDES-connectorserver probeer te installeren, krijg ik het bericht: "Het wachtwoord in het certificaatverzoek kan niet worden geverifieerd. Het kan al gebruikt zijn. Een nieuw wachtwoord aanvragen om met dit verzoek in te dienen."**  

Dit bericht betekent dat u de installatie van de certificaatconnector als administrator moet uitvoeren.

In sommige omgevingen moeten de servers waarop het Intune-certificaat wordt uitgevoerd, een proxyserver gebruiken om verbinding te maken met Intune, zodat de Certificate Connector een proxy moet gebruiken. In sommige gevallen negeert de NDES-connector de geconfigureerde proxy-instellingen en is het mogelijk dat de proxy-instellingen tijdens het uitvoeren in de beveiligingscontext van LocalSystem moeten worden geconfigureerd. 
 
De oplossing is om Internet Explorer als SYSTEEM uit te voeren en een proxy in IE te configureren. Na een herstart van de Intune Connector Service maakt de NDES Connector verbinding met Intune.

**Gebruikersapparaten ontvangen geen SCEP-certificaten meer van NDES.**

Het is mogelijk dat het certificaat voor clientverificatie dat is afgegeven aan de NDES-server en is opgegeven tijdens de installatie van de NDES-connector, is verlopen of ontbreekt. Ga als een oplossing voor: 
 
1. Verwijder de NDES-connector.  
2. Gebruik deze gegevens om een nieuw certificaat voor clientverificatie of serververificatie aan te vragen: 
 
    - Onderwerpnaam: CN=external fqdn  
    - Onderwerp alternatieve naam (beide zijn vereist): DNS=externe fqdn, DNS=internal fqdn 
 
3. Installeer de NDES-connector opnieuw met het nieuwe certificaat.