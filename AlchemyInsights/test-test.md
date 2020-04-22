---
title: Ontbrekende termen in SharePoint Online-termenarchief
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766848"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker-versleuteling inschakelen met Intune

Intune Endpoint Protection Policy kan worden gebruikt om De encryptie-instellingen van Boitlocker voor Windows-apparaten te configureren, zoals beschreven in : Windows10 (en hoger) instellingen om apparaten te beschermen met Behulp van Intune

U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische bitlocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van het MDM-beleid. Dit kan gevolgen hebben voor de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd. Zie veelgestelde vragen voor meer informatie.


FAQ  Q: Welke edities van Windows-ondersteuning apparaat encryptie met behulp van het Endpoint Protection Policy?
 A: De instellingen in het Intune Endpoint Protection Policy worden geïmplementeerd met de Bitlocker CSP.Niet alle edities, noch builds van Windows ondersteunen de Bitlocker CSP. 
      Op dit moment Windows Editions: Enterprise; Onderwijs, Mobiel, Mobiel Ondernemen en Professional (vanaf build 1809) worden ondersteund.




V: Als een apparaat al is versleuteld met Bitlocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en versleutelingssterkte (XTS-AES-128) zal het toepassen van een beleid met verschillende instellingen automatisch leiden tot re-encryptie van het station met de nieuwe instellingen?

A: Nee. Om de nieuwe cijferinstellingen toe te passen moet het station eerst worden gedecodeerd.

Opmerking Voor apparaten die zijn ingeschreven bij Autopilot wordt de automatische versleuteling die tijdens OOBE zou optreden, pas geactiveerd nadat het Intune-beleid is geëvalueerd, waardoor de beleidsgebaseerde instellingen kunnen worden gebruikt in plaats van de standaardinstellingen van het besturingssysteem




V Als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid zal het worden gedecodeerd wanneer dat beleid wordt verwijderd?

A: Verwijdering van encryptie gerelateerde beleid niet resulteren in decryptie van de stations die zijn geconfigureerd.




V: Waarom laat het intune Compliance-beleid zien dat mijn apparaat geen "Bitlocker Enabled" heeft, maar dat is het wel?

A: De instelling 'Bitlocker ingeschakeld' in het nalevingsbeleid intune maakt gebruik van de DHA-client (Windows Device Health Attestation). Deze client meet alleen de apparaatstatus bij het opstarten. Dus als een apparaat niet opnieuw is opgestart sinds bitlocker encryptie is voltooid de DHA client service zal niet bitlocker melden als actief.