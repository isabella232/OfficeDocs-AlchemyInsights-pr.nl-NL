---
title: Office-apps repareren Sorry, we hebben een tijdelijke server problemen bericht
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627985"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Het oplossen van de Office-apps ' Sorry, we hebben tijdelijke server problemen ' bericht

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