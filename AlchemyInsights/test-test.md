---
title: Voorwaarden ontbreken in SharePoint Online term Store
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762051"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-versleuteling inschakelen met intune

InTune Endpoint Protection-beleid kan worden gebruikt voor het configureren van Boitlocker-versleutelingsinstellingen voor Windows-apparaten zoals beschreven in: Windows10 (en latere) instellingen om apparaten te beveiligen met behulp van intune

U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van MDM-beleid. Dit kan invloed hebben op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd. Zie de veelgestelde vragen voor meer informatie.


Veelgestelde  vragen over Q: welke edities van Windows ondersteuning voor apparaatversleuteling met behulp van het Endpoint Protection-beleid?
 A: de instellingen in intune Endpoint Protection-beleid worden geïmplementeerd met behulp van de BitLocker-CSP.Niet alle edities of builds van Windows ondersteunen de BitLocker-CSP. 
      Op dit moment Windows-edities: Enterprise; Onderwijs, mobiel, mobiel ondernemen en professioneel (vanaf build 1809) worden ondersteund.




V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en codeersterkte (XTS-AES-128) zal een beleid met verschillende instellingen automatisch opnieuw versleutelen van het station activeren met de nieuwe instellingen?

A: Nee. Om de nieuwe cipher instellingen toe te passen moet het station eerst worden gedecodeerd.

Opmerking voor apparaten die worden ingeschreven met de stuurautomaat de automatische versleuteling die tijdens OOBE optreden wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, waardoor de beleidsinstellingen die kunnen worden gebruikt in plaats van de standaardwaarden van het besturingssysteem




V als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid wordt deze ontsleuteld wanneer dat beleid wordt verwijderd?

A: verwijdering van versleuteling gerelateerd beleid leidt niet tot ontsleuteling van de stations die zijn geconfigureerd.




V: Waarom laat het nalevingsbeleid van intune zien dat mijn apparaat geen ' BitLocker ingeschakeld ' heeft, maar wel?

A: de instelling ' BitLocker ingeschakeld ' in het nalevingsbeleid van intune maakt gebruik van de Windows Device Health Attestation (DHA)-client. Deze client meet alleen de apparaatstatus tijdens het opstarten. Dus als een apparaat niet opnieuw is opgestart sinds BitLocker-versleuteling is voltooid de DHA-client service wordt BitLocker niet rapporteren als actief.