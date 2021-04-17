---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815610"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker-versleuteling inschakelen met Intune

Intune Endpoint Protection Policy kan worden gebruikt voor het configureren van Bitlocker-versleutelingsinstellingen voor Windows-apparaten. Zie Windows [10 (en hoger)](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)instellingen voor het beveiligen van apparaten met Intune voor meer informatie.

Naast het endpointbeveiligingsbeleid is er ook een versleutelingsrapport dat een gedetailleerdere weergave biedt van de versleutelingsstatus voor apparaten. Dit rapport kan worden geopend vanuit de MEM-portal onder **Apparaten > Monitor** en vervolgens onder **Configuratie** selecteer [Versleutelingsrapport](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Als u vindt dat Bitlocker niet is ingeschakeld zoals verwacht of als het profiel dat wordt gebruikt om Bitlocker in te stellen een fouttoestand heeft, raadpleegt u het versleutelingsrapport om beter te begrijpen waarom het gedrag optreedt.

Zie Apparaatversleuteling controleren met [Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)voor meer informatie over het interpreteren van het rapport, inclusief de verschillende waarden voor versleutelingsstatus.

U moet er rekening mee houden dat veel nieuwere apparaten met Windows 10 automatische Bitlocker-versleuteling ondersteunen, die wordt geactiveerd zonder de toepassing van MDM-beleid. Dit kan van invloed zijn op de toepassing van beleid als niet-standaardinstellingen zijn geconfigureerd. Zie de volgende veelgestelde vragen voor meer informatie.

Zie BitLocker-beleid in Microsoft Intune oplossen voor informatie over het oplossen van [bitlockerproblemen.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Veelgestelde vragen**

V: Welke versies van Windows ondersteunen apparaatversleuteling met het endpointbeveiligingsbeleid?<br>
A: De instellingen in het Intune Endpoint Protection Policy worden geïmplementeerd met de [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Niet alle versies of builds van Windows ondersteunen de Bitlocker CSP. <br><br>

V: Hoe kan Bitlocker worden ingeschakeld op apparaten zonder tussenkomst van de eindgebruiker?<br>
A: Zolang aan de vereiste vereisten wordt voldaan, kunt u Bitlocker 'Silent Encryption' inschakelen via Intune. Zie de details van de apparaatvereisten en voorbeeldbeleidsinstellingen voor het inschakelen van stille versleuteling in het volgende document: Bitlockerversleuteling stil [inschakelen.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

V: Als een apparaat al is versleuteld met Bitlocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en codeersterkte (XTS-AES-128), wordt er automatisch een beleid met verschillende instellingen toegepast waarmee de versleuteling van het station automatisch wordt geactiveerd met de nieuwe instellingen?<br>
A: Nee. Als u de nieuwe coderingsinstellingen wilt toepassen, moet het station eerst worden ontsleuteld.<br><br>
**Opmerking:** Voor apparaten die zijn geregistreerd met Autopilot, wordt de automatische versleuteling die zou plaatsvinden tijdens OOBE pas geactiveerd als het Intune-beleid is geëvalueerd, zodat de beleidsinstellingen kunnen worden gebruikt in plaats van de standaardinstellingen van het besturingssysteem.
 
V: Als een apparaat is versleuteld als gevolg van de toepassing van het Intune-beleid, wordt het dan ontsleuteld wanneer dat beleid wordt verwijderd?<br>
A: Verwijdering van versleutelingsgerelateerde beleid resulteert NIET in ontsleuteling van de stations die zijn geconfigureerd.
 
V: Waarom wordt in het Compliancebeleid van Intune laten zien dat bitlocker op mijn apparaat niet is ingeschakeld, ook al is dat zo?<br>
A: De instelling 'Bitlocker enabled' in de Intune Compliance Policy maakt gebruik van de Windows Device Health Attestation (DHA) client. Deze client meet alleen de apparaattoestand tijdens het opstarten. Dus als een apparaat niet opnieuw is opgestart sinds Bitlocker-versleuteling is voltooid, wordt Bitlocker niet als actief door de DHA-clientservice rapporteren.
 
 