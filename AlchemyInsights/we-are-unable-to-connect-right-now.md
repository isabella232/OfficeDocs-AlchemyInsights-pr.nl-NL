---
title: Activeringsprobleem-we kunnen nu geen verbinding maken
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628237"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>De Office-apps repareren "we kunnen nu geen verbinding maken" bericht

Als dit bericht wordt weergegeven, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te bevestigen dat ze Internet toegang tot Office-apps niet blokkeren. Zie [Office 365-url's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga naar **Start** > **uitvoeren**, en typ vervolgens **Services. msc**. Zorg ervoor dat de volgende services worden uitgevoerd:
    - Netwerk verbonden apparaten Auto-Setup
    - Network List service
    - Netwerklocatie bewustzijn
    - Windows-gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem ondervindt bij het starten van de service, voert u de volgende opdracht uit door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc/scannow**

Start de computer opnieuw op nadat deze opdracht is voltooid.

Zie [' Sorry, we kunnen geen verbinding maken met uw account ' voor gedetailleerde informatie. Probeer het later opnieuw ' fout bij het activeren van Office van Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).