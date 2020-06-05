---
title: Microsoft 365-apps oplossen Sorry, we hebben een bericht over tijdelijke serverproblemen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582698"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Het bericht microsoft 365-apps 'Sorry, we hebben tijdelijke serverproblemen' oplossen

Als u dit bericht ontvangt, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Microsoft 365-apps niet blokkeren. Zie [URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga **Start**naar  >  **Start Run**en typ **services.msc**. Controleer of de volgende services allemaal worden uitgevoerd:
    - Netwerkgekoppelde apparaten automatisch instellen
    - Netwerklijstservice
    - Netwerklocatiebewustzijn
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is voltooid, start u de computer opnieuw.

Zie ['Sorry, we kunnen geen verbinding maken met je account voor meer informatie. Probeer het later opnieuw" fout wanneer u activeert](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).