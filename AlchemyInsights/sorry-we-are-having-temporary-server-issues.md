---
title: Problemen met Microsoft 365 oplossen Sorry, er zijn tijdelijke serverproblemen
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021591"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Het oplossen Microsoft 365 apps 'Sorry, we hebben tijdelijke serverproblemen' bericht

Als u dit bericht ontvangt, gaat u als volgt te werk:

1. Controleer de firewall-, antivirussoftware- en proxy-instellingen om te bevestigen dat ze de toegang tot internet tot Microsoft 365 blokkeren. Zie [URL's en IP-adresbereiken.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Ga naar **Start**  >  **Run** en typ **services.msc**. Zorg ervoor dat de volgende services worden uitgevoerd:
    - Auto-setup van verbonden netwerkapparaten
    - Netwerklijstservice
    - Netwerklocatiebekendheid
    - Windows Gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, kunt u de volgende opdracht uitvoeren door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is klaar, start u de computer opnieuw op.

Zie 'Sorry, we kunnen geen verbinding maken met uw account' voor [meer informatie. Probeer het later opnieuw' fout wanneer u activeert.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)