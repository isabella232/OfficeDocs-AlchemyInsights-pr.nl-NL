---
title: Office-apps oplossen Helaas hebben we een bericht over tijdelijke serverproblemen
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764112"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Het bericht 'Sorry, we hebben tijdelijke serverproblemen'

Als u dit bericht ontvangt, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Office-apps niet blokkeren. Zie [URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga naar **Run** > **starten**en typ **services.msc**. Controleer of de volgende services allemaal worden uitgevoerd:
    - Netwerkverbonden apparaten automatisch instellen
    - Netwerklijstservice
    - Netwerklocatiebewustzijn
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is voltooid, start u de computer opnieuw op.

Zie ['Sorry, we kunnen geen verbinding maken met uw account' voor meer informatie. Probeer het later opnieuw" fout wanneer u activeert](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).