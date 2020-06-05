---
title: Problemen met gebeurtenissen oplossen via e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569006"
---
# <a name="troubleshooting-events-from-email"></a>Problemen met gebeurtenissen oplossen via e-mail

1. Controleer of de functie is ingeschakeld voor het postvak: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Kijk dan naar de 'Gebeurtenissen uit e-mail' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Zoek in de logboeken 'Gebeurtenissen uit e-mail' de InternetMessageId die overeenkomt met het item in het postvak.  

4. De TrustScore bepaalt of het item is toegevoegd of niet. Gebeurtenissen worden alleen toegevoegd als de TrustScore = "Vertrouwd" wordt.

De TrustScore wordt bepaald door de eigenschappen SPF, Dkim of Dmarc, die zich in de berichtkoptekst bevinden.

Ga als u deze eigenschappen wilt bekijken:

**Bureaublad Outlook**

- Het item openen
- Bestands -> Eigenschappen -> internetkoppen

of

**MFCMapi MFCMapi**

- Navigeren naar het item in het postvak IN
- Zoek naar PR_TRANSPORT_MESSAGE_HEADERS_W

Deze eigenschappen worden bepaald en geregistreerd tijdens transport en routing. Voor verdere probleemoplossing moet u mogelijk de transportondersteuning opvolgen over de fouten in SPF, DKIM en.or DMARC.