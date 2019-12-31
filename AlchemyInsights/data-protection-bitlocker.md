---
title: Data Provider-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908705"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-versleuteling inschakelen met intune

 InTune Endpoint Protection-beleid kan worden gebruikt voor het configureren van BitLocker-versleutelingsinstellingen voor Windows-apparaten. Zie voor meer informatie [instellingen voor Windows 10 (en hoger) om apparaten te beveiligen met intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen, die wordt geactiveerd zonder de toepassing van MDM-beleid. Dit kan invloed hebben op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd. Zie de volgende veelgestelde vragen voor meer informatie.
 
Zie [problemen met BitLocker-beleid in Microsoft intune oplossen](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)voor meer informatie over het oplossen van problemen met BitLocker.
 
 
**Veelgestelde vragen**

 V: welke edities van Windows ondersteuning voor apparaatversleuteling met behulp van het Endpoint Protection-beleid?<br>
 A: de instellingen in intune Endpoint Protection-beleid worden geïmplementeerd met behulp van de [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Niet alle edities of builds van Windows ondersteunen de BitLocker-CSP. <br><br>
      Op dit moment worden de volgende Windows-edities ondersteund: Enterprise, education, Mobile, Mobile Enterprise en Professional (build 1809 en hoger).
 
V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en codeersterkte (XTS-AES-128), zal een beleid met verschillende instellingen automatisch opnieuw versleutelen van het station activeren met de nieuwe instellingen?<br>
A: Nee. Als u de nieuwe coderingsinstellingen wilt toepassen, moet het station eerst worden ontsleuteld.<br><br>
**Opmerking:** Voor apparaten die worden ingeschreven met Autopilot, wordt de automatische versleuteling die tijdens OOBE optreden wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, waardoor de op beleid gebaseerde instellingen kunnen worden gebruikt in plaats van de standaardwaarden van het besturingssysteem.
 
V: als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid, wordt deze ontsleuteld wanneer dat beleid wordt verwijderd?<br>
A: het verwijderen van beleid met betrekking tot versleuteling leidt niet tot ontsleuteling van de stations die zijn geconfigureerd.
 
V: Waarom wordt in het nalevingsbeleid van intune weergegeven dat BitLocker niet is ingeschakeld op mijn apparaat, ook al is het?<br>
A: de instelling ' BitLocker ingeschakeld ' in het nalevingsbeleid van intune maakt gebruik van de Windows Device Health Attestation (DHA)-client. Deze client meet alleen de apparaatstatus tijdens het opstarten. Dus als een apparaat niet opnieuw is opgestart sinds BitLocker-versleuteling is voltooid, de DHA-client service wordt BitLocker niet rapporteren als actief.
 
 