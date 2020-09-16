---
title: Activerings probleem – we kunnen momenteel geen verbinding maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725978"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Bericht over het herstellen van de Microsoft 365-apps ' we kunnen nu geen verbinding maken '

Als dit bericht wordt weergegeven, probeert u het volgende:

1. Controleer uw firewall, antivirussoftware en proxy-instellingen om te controleren of de Internet toegang tot Microsoft 365-apps niet wordt geblokkeerd. Zie [url's en IP-adresbereiken voor Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ga naar **Start**  >  **Run**en typ **Services. msc**. Zorg dat de volgende services allemaal worden uitgevoerd:
    - Automatisch instellen met netwerk verbonden apparaten
    - Service voor netwerk lijsten
    - Bewustmaking van netwerklocatie
    - Gebeurtenissenlogboek van Windows

Als een van deze services niet actief is, probeert u het programma te starten. Als u problemen ondervindt bij het starten van de service, voert u de volgende opdracht uit als u een opdrachtprompt opent met verhoogde machtigingen:

**sfc/scannow**

Start de computer opnieuw op nadat u deze opdracht hebt voltooid.

Voor meer informatie raadpleegt [u ' Sorry, we kunnen geen verbinding maken met uw account. Probeer het later opnieuw "wanneer u Office activeert bij Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).