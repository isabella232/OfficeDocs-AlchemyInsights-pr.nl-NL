---
title: Activeringsprobleem - We kunnen op dit moment geen verbinding maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581870"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Vaststelling van de Microsoft 365 apps "We zijn niet in staat om verbinding te maken op dit moment" bericht

Als u dit bericht ontvangt, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Microsoft 365-apps niet blokkeren. Zie [Microsoft URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga **Start**naar  >  **Start Run**en typ **services.msc**. Controleer of de volgende services allemaal worden uitgevoerd:
    - Netwerkgekoppelde apparaten automatisch instellen
    - Netwerklijstservice
    - Netwerklocatiebewustzijn
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is voltooid, start u de computer opnieuw.

Zie ['Sorry, we kunnen geen verbinding maken met je account voor meer informatie. Probeer het later opnieuw" fout wanneer u Office activeert vanuit Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).