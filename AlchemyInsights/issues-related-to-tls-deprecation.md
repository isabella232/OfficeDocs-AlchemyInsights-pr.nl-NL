---
title: Kan geen e-mail verzenden/ontvangen van/naar Office 365 vanwege de TLS 1.0- en TLS 1.1-uitschakelen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743970"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Kan geen e-mail verzenden/ontvangen van/naar Office 365 vanwege de TLS 1.0- en TLS 1.1-uitschakelen

Zoals bevestigd door het berichtcentrum na MC229914, zijn de intrekking van TLS 1.0 en TLS 1.1 gestart met het afdwingen van exchange Online-eindpunten voor e-mailstroom. Office 365 accepteert binnenkort geen E-mailverbindingen van TLS 1.0 en TLS 1.1 meer vanuit externe bronnen. Exchange Online gebruikt ook nooit TLS 1.0 of 1.1 om uitgaande e-mail te verzenden. Als er problemen optreden vanwege TLS 1.0 of 1.1-uitschakelen, kan er een van de volgende fouten optreden.

- Afzender krijgt NDR-bounce terug - '421 4.4.2 Connection dropped due to SocketError'
- Fout in de wachtrijviewer van on-premises server die e-mail verstuurt naar Officer 365- '421 4.4.2 Connection dropped due to SocketError'
- Fout in Protocollogboek [verbindingslijn verzenden](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) op de server die e-mail verzendt naar Office 365- TLS-onderhandeling is mislukt met fout SocketError
- Fout in Protocollogboek Verbindingslijn verzenden of ontvangen - '451 5.7.3 Moet eerst een STARTTLS-opdracht geven'

Als u een van de bovenstaande fouten ervaart, controleert u of TLS 1.2 is ingeschakeld op de server die e-mail verstuurt of ontvangt door de volgende registersleutels te controleren.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Als u de bovenstaande registersleutels wijzigt om TLS 1.2 in te stellen, start u de server opnieuw op om de wijzigingen van kracht te laten worden. Zorg er ook voor dat u de nieuwste Windows- en Exchange-updates hebt geïnstalleerd.

Zie voor meer informatie:

- [Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Informatie over e-mailscenario's als TLS-versies niet kunnen worden overeengekomen met Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
