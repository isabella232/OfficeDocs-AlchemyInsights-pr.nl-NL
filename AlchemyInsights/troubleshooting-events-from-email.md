---
title: Problemen met gebeurtenissen vanuit e-mail oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834834"
---
# <a name="troubleshooting-events-from-email"></a>Problemen met gebeurtenissen vanuit e-mail oplossen

1. Controleer of de functie is ingeschakeld voor het postvak: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Bekijk vervolgens de logboeken 'Gebeurtenissen uit e-mail' **Export-MailboxDiagnosticLogs<mailbox> -Component TimeProfile**

3. Zoek in de logboeken 'Gebeurtenissen uit e-mail' de InternetMessageId die overeenkomt met het item in het postvak.  

4. De TrustScore bepaalt of het item wordt toegevoegd of niet. Gebeurtenissen worden alleen toegevoegd als de TrustScore = 'Trusted'.

De TrustScore wordt bepaald door de SPF-, Dkim- of Dmarc-eigenschappen, die in de berichtkop staan.

Om deze eigenschappen te bekijken:

**Bureaubladversie van Outlook**

- Het item openen
- Bestand -> Eigenschappen -> Internetkoppen

of

**MFCMapi**

- Naar het item in het Postvak IN gaan
- Zoek naar PR_TRANSPORT_MESSAGE_HEADERS_W

Deze eigenschappen worden bepaald en vastgelegd tijdens transport en routering. Voor verdere probleemoplossing moet u mogelijk contact opnemen met Transport Support over de fouten in SPF, DKIM en/of DMARC.