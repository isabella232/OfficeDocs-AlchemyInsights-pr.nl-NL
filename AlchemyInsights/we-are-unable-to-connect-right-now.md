---
title: Activeringsprobleem - We kunnen nu geen verbinding maken
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716167"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Het bericht 'We kunnen nu geen verbinding maken' herstellen in de Office-apps

Als u dit bericht ontvangt, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze de internettoegang tot Office-apps niet blokkeren. Zie [Url's en IP-adresbereiken van Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga naar **Run** > **starten**en typ **services.msc**. Controleer of de volgende services allemaal worden uitgevoerd:
    - Netwerkverbonden apparaten automatisch instellen
    - Netwerklijstservice
    - Netwerklocatiebewustzijn
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is voltooid, start u de computer opnieuw op.

Zie ['Sorry, we kunnen geen verbinding maken met uw account' voor meer informatie. Probeer het later opnieuw" fout wanneer u Office activeert vanuit Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).