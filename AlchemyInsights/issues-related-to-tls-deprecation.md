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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="29d2d-102">Kan geen e-mail verzenden/ontvangen van/naar Office 365 vanwege de TLS 1.0- en TLS 1.1-uitschakelen</span><span class="sxs-lookup"><span data-stu-id="29d2d-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="29d2d-103">Zoals bevestigd door het berichtcentrum na MC229914, zijn de intrekking van TLS 1.0 en TLS 1.1 gestart met het afdwingen van exchange Online-eindpunten voor e-mailstroom.</span><span class="sxs-lookup"><span data-stu-id="29d2d-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="29d2d-104">Office 365 accepteert binnenkort geen E-mailverbindingen van TLS 1.0 en TLS 1.1 meer vanuit externe bronnen.</span><span class="sxs-lookup"><span data-stu-id="29d2d-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="29d2d-105">Exchange Online gebruikt ook nooit TLS 1.0 of 1.1 om uitgaande e-mail te verzenden.</span><span class="sxs-lookup"><span data-stu-id="29d2d-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="29d2d-106">Als er problemen optreden vanwege TLS 1.0 of 1.1-uitschakelen, kan er een van de volgende fouten optreden.</span><span class="sxs-lookup"><span data-stu-id="29d2d-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="29d2d-107">Afzender krijgt NDR-bounce terug - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="29d2d-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="29d2d-108">Fout in de wachtrijviewer van on-premises server die e-mail verstuurt naar Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="29d2d-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="29d2d-109">Fout in Protocollogboek [verbindingslijn verzenden](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) op de server die e-mail verzendt naar Office 365- TLS-onderhandeling is mislukt met fout SocketError</span><span class="sxs-lookup"><span data-stu-id="29d2d-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="29d2d-110">Fout in Protocollogboek Verbindingslijn verzenden of ontvangen - '451 5.7.3 Moet eerst een STARTTLS-opdracht geven'</span><span class="sxs-lookup"><span data-stu-id="29d2d-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="29d2d-111">Als u een van de bovenstaande fouten ervaart, controleert u of TLS 1.2 is ingeschakeld op de server die e-mail verstuurt of ontvangt door de volgende registersleutels te controleren.</span><span class="sxs-lookup"><span data-stu-id="29d2d-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="29d2d-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="29d2d-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="29d2d-113">Als u de bovenstaande registersleutels wijzigt om TLS 1.2 in te stellen, start u de server opnieuw op om de wijzigingen van kracht te laten worden.</span><span class="sxs-lookup"><span data-stu-id="29d2d-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="29d2d-114">Zorg er ook voor dat u de nieuwste Windows- en Exchange-updates hebt geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="29d2d-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="29d2d-115">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="29d2d-115">For more information, see:</span></span>

- [<span data-ttu-id="29d2d-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="29d2d-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="29d2d-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="29d2d-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="29d2d-118">Informatie over e-mailscenario's als TLS-versies niet kunnen worden overeengekomen met Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="29d2d-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
