---
title: Kan het AllowSelfServicePurchase-beleid niet instellen of bekijken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091686"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan het AllowSelfServicePurchase-beleid niet instellen of bekijken

Wanneer u het allowselfservice-aankoopbeleid probeert in te stellen of weer te geven, ontvangt u het volgende foutbericht:

*HandleError : Kan het productbeleid niet ophalen met PolicyId 'AllowSelfServicePurchase', ErrorMessage - De onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden op een verzenden.*

Dit kan te wijten zijn aan een oudere versie van Transport Layer Security (TLS). Als u de MSCommerce-service wilt aansluiten, moet u TLS 1.2 of hoger gebruiken.  

Probeer de volgende stappen om het TLS-protocol in te schakelen/in te stellen op 1.2, te verifiëren en opnieuw te proberen.
 1. Voer bij de opdrachtprompt van\) PowerShell (PS C: voer de volgende opdracht in om het TLS-protocol in te stellen op versie 1.2:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Controleer het gebruikte TLS-protocol(en) met de volgende opdracht:

    \[Net.ServicePointManager]::SecurityProtocol 

3. Probeer de opdrachten Get of Update indien nodig opnieuw.

