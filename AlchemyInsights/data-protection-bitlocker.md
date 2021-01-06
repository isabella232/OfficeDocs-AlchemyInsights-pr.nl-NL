---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768812"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-versleuteling inschakelen met intune

 Het beleid voor het intune-endpoint voor beveiliging kan worden gebruikt voor het configureren van BitLocker-versleutelingsinstellingen voor Windows-apparaten. Zie voor meer informatie de [instellingen van Windows 10 (en later) om apparaten te beschermen met intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
U dient te beseffen dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen, die wordt geactiveerd zonder de toepassing van MDM-beleid. Dit kan van invloed zijn op de toepassing van beleid als niet-standaardinstellingen zijn geconfigureerd. Zie de volgende veelgestelde vragen voor meer informatie.
 
Voor informatie over het oplossen van problemen met BitLocker, raadpleegt u [problemen met BitLocker-beleid in Microsoft intune oplossen](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Veelgestelde vragen**

V: welke versies van Windows ondersteunen apparaatversleuteling met het Endpoint Protection-beleid?<br>
A: de instellingen in intune-Endpoint Protection-beleid worden geïmplementeerd met de [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Niet alle edities of versies van Windows ondersteunen de BitLocker CSP. <br><br>

V: hoe kan BitLocker worden ingeschakeld op apparaten zonder dat de interactie met eindgebruikers is vereist?<br>
A: zo lang de noodzakelijke voorwaarden zijn aan te passen, kunt u BitLocker ' stille versleuteling ' inschakelen via intune. Zie de details van de hardwarevereisten en de voorbeeld beleidsinstellingen voor het inschakelen van de Stille versleuteling in het volgende document: [BitLocker-versleuteling](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)op de achtergrond inschakelen. <br><br>

V: als een apparaat al met BitLocker is versleuteld met de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en versleutelingssterkte (XTS-AES-128), wordt een beleid toegepast met andere instellingen om het station automatisch opnieuw te versleutelen met de nieuwe instellingen?<br>
A: Nee. Als u de nieuwe versleutelingsinstellingen wilt toepassen, moet het station eerst worden gedecodeerd.<br><br>
**Opmerking:** Voor apparaten die met auto pilot worden ingeschreven, wordt de automatische versleuteling die zich in OOBE voordoet, niet geactiveerd totdat het intune-beleid wordt geëvalueerd, zodat de instellingen op basis van het beleid kunnen worden gebruikt in plaats van de standaardinstellingen van het besturingssysteem.
 
V: als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid, wordt deze gedecodeerd wanneer dat beleid wordt verwijderd?<br>
A: het verwijderen van het versleutelingsbeleid veroorzaakt geen decodering van de stations die zijn geconfigureerd.
 
V: Waarom wordt in het nalevingsbeleid van intune aangegeven dat mijn apparaat BitLocker niet heeft ingeschakeld, ook niet als dit is?<br>
A: de instelling ' BitLocker ingeschakeld ' in het intune-nalevingsbeleid maakt gebruik van de client (DHA) voor Windows-apparaatstatusverklaring. Dit is alleen van toepassing op de status van het apparaat tijdens het opstarten. Als een apparaat na voltooiing van BitLocker-versleuteling niet opnieuw is opgestart, meldt de DHA client service geen BitLocker als actief.
 
 