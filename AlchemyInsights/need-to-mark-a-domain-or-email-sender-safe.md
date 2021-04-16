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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792127"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Wilt u een domein of e-mail afzender veilig markeren?

- Het gebruik **van lijsten met veilige afzenders wordt** niet aanbevolen, omdat uw organisatie hiermee wordt geopend voor spam-, phish- en spoofing-aanvallen.
- Als er echter een zakelijke vereiste is, **raden** we u aan hiervoor **[E-mailstroomregels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken. Onze richtlijnen zorgen ervoor dat afzenderverificatie (controleert of verzendend domein niet wordt vervalst). **Opmerking:** Het is niet raadzaam om false positives te beheren met behulp van lijsten met veilige afzenders, omdat uitzonderingen op spamfilters uw organisatie kunnen openen voor beveiligingsaanvallen. Als uw gebruikers berichten ontvangen die onjuist zijn gemarkeerd als spam of ongewenste e-mail, kunt u berichten en bestanden **[rapporteren aan Microsoft.](https://protection.office.com/reportsubmission)**
- Veilige afzenders in Outlook, lijst met toegestane afzenders  of toegestane domeinlijst in antispambeleid moeten worden vermeden omdat afzenders alle spam-, spoof- en phish-beveiliging en afzenderverificatie (SPF, DKIM, DMARC) omzeilen. Deze methode wordt het beste alleen gebruikt voor tijdelijke tests.
