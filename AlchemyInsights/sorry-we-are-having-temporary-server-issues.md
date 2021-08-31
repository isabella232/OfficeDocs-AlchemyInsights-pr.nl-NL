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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744641"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Het oplossen Microsoft 365 apps 'Sorry, er zijn tijdelijke serverproblemen' bericht

Opmerking: Als u een oudere versie van Windows gebruikt (bijvoorbeeld Windows 7 SP1, Windows Server 2008 R2), gebruikt u de eenvoudige oplossing om TLS 1.2 standaard in te stellen. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Zie Bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)in te stellen als standaardveilige protocollen in WinHTTP in Windows.

Als u dit bericht ontvangt, gaat u als volgt te werk:

1. Controleer uw firewall-, antivirussoftware- en proxy-instellingen om te bevestigen dat ze geen internetverbinding blokkeren voor Microsoft 365 apps. Zie [URL's en IP-adresbereiken.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Ga naar **Start**  >  **Run** en typ **services.msc.** Zorg ervoor dat de volgende services worden uitgevoerd:
    - Auto-setup van verbonden apparaten met netwerk
    - Netwerklijstservice
    - Netwerklocatiebekendheid
    - Windows Gebeurtenislogboek

Als een van deze services niet wordt uitgevoerd, probeert u deze te starten. Als u een probleem hebt met het starten van de service, kunt u de volgende opdracht uitvoeren door een opdrachtprompt met verhoogde machtigingen te openen:

**sfc /scannow**

Nadat deze opdracht is klaar, start u de computer opnieuw op.

Zie 'Sorry, we kunnen geen verbinding maken met uw account' voor [meer informatie. Probeer het later opnieuw' fout wanneer u activeert.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)