---
title: Kan het beleid AllowSelfServicePurchase niet instellen of weergeven
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826086"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan het beleid AllowSelfServicePurchase niet instellen of weergeven

Wanneer u het beleid AllowSelfServicePurchase probeert in te stellen of weer te geven, ontvangt u het volgende foutbericht:

*HandleError: Kan het productbeleid niet ophalen met PolicyId 'AllowSelfServicePurchase', ErrorMessage - De onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden bij een verzenden.*

Dit kan het gevolg zijn van een oudere versie van Transport Layer Security (TLS). Als u verbinding wilt maken met de MSCommerce-service, moet u TLS 1.2 of hoger gebruiken.  

Probeer de volgende stappen om het TLS-protocol in te stellen op 1.2, te verifiëren en opnieuw te proberen.
 1. Voer bij de Opdrachtprompt van PowerShell (PS C: voer de volgende opdracht in om het TLS-protocol in te stellen \) op versie 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Controleer het TLS-protocol(en) dat in gebruik is, met de volgende opdracht:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. U kunt de opdrachten Downloaden of Bijwerken zo nodig opnieuw proberen.

