---
title: Kan het AllowSelfServicePurchase-beleid niet instellen of weergeven
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735194"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan het AllowSelfServicePurchase-beleid niet instellen of weergeven

Wanneer u probeert het AllowSelfServicePurchase-beleid in te stellen of weer te geven, wordt het volgende foutbericht weergegeven:

*HandleError: kan geen productbeleid ophalen met PolicyId ' AllowSelfServicePurchase ', ErrorMessage-de onderliggende verbinding is gesloten: er is een onverwachte fout opgetreden bij het verzenden.*

Dit kan zijn vanwege een oudere versie van TLS (Transport Layer Security). U moet TLS 1,2 of hoger gebruiken om verbinding te maken met de MSCommerce-service.  

Voer de volgende stappen uit om het TLS-protocol in te stellen op 1,2, Controleer en probeer het opnieuw.
 1. Bij de PowerShell-opdrachtprompt (PS C: \) Voer de volgende opdracht in om het TLS-protocol in te stellen op versie 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Controleer de TLS-protocol (s) die u gebruikt, met de volgende opdracht:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Voer de opdrachten voor het uitvoeren of bijwerken naar wens opnieuw.

