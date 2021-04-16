---
title: 'Activeringsprobleem: we kunnen momenteel geen verbinding maken'
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806437"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Fix the Microsoft 365 apps "We are unable to connect right now" bericht

Als u dit bericht ontvangt, gaat u als volgt te werk:

1. Controleer uw firewall-, antivirussoftware- en proxy-instellingen om te bevestigen dat ze geen internetverbinding blokkeren voor Microsoft 365-apps. Zie [Microsoft URL's en IP-adresbereiken.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Ga naar **Start**  >  **Run** en typ **services.msc**. Zorg ervoor dat de volgende services worden uitgevoerd:
    - Auto-setup van verbonden netwerkapparaten
    - Netwerklijstservice
    - Netwerklocatiebekendheid
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, kunt u de volgende opdracht uitvoeren door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is klaar, start u de computer opnieuw op.

Zie 'Sorry, we kunnen geen verbinding maken met uw account' voor [meer informatie. Probeer het later opnieuw' fout wanneer u Office activeert vanuit Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)