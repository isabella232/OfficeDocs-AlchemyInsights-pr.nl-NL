---
title: Wilt u een domein of e-mail afzender veilig markeren?
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
- "9002921"
- "5673"
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025605"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Wilt u een domein of e-mail afzender veilig markeren?

- Het gebruik **van lijsten met veilige afzenders wordt** niet aanbevolen, omdat uw organisatie hiermee wordt geopend voor spam-, phish- en spoofing-aanvallen.
- Als er echter een zakelijke vereiste is, **raden** we u aan mail **[Flow hiervoor](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken. Onze richtlijnen zorgen ervoor dat afzenderverificatie (controleert of verzendend domein niet wordt vervalst). **Opmerking:** Het is niet raadzaam om false positives te beheren met behulp van lijsten met veilige afzenders, omdat uitzonderingen op spamfilters uw organisatie kunnen openen voor beveiligingsaanvallen. Als uw gebruikers berichten ontvangen die onjuist zijn gemarkeerd als spam of ongewenste e-mail, kunt u berichten en bestanden **[rapporteren aan Microsoft.](https://protection.office.com/reportsubmission)**
- Safe Afzenders in Outlook, lijst met toegestane afzenders of  toegestane domeinlijst in antispambeleid moeten worden vermeden, omdat afzenders alle spam-, spoof- en phish-beveiliging en afzenderverificatie (SPF, DKIM, DMARC) omzeilen. Deze methode wordt het beste alleen gebruikt voor tijdelijke tests.
- De validatie dat een bepaalde e-mail Antispam-evaluatie heeft overgeslagen, kan worden uitgevoerd door de berichtkop 'X-Forefront-Antispam-Report' (SFV:SFE, SFV:SKA, SFV:SKN) te controleren, zie Kopteksten van **[antispamberichten.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Omdat Microsoft onze klanten standaard veilig wil [houden,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)worden sommige tenant-overschrijvingen niet toegepast op malware en phishing met veel vertrouwen. Deze overschrijven zijn: o Toegestane afzenderlijsten of toegestane domeinlijsten (antispambeleid) o Outlook Safe Senders o IP Allow List (verbindingsfiltering) 
- De enige overschrijven die phishing met veel vertrouwen mogelijk maakt om filteren te omzeilen, is Exchange regels voor e-mailflow (ook wel transportregels genoemd). Zie Regels voor e-mailstroom gebruiken om het filteren te omzeilen door E-mailstroomregels te gebruiken om het betrouwbaarheidsniveau **[voor spam (SCL) in berichten in te stellen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**