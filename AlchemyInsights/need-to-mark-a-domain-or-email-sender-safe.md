---
title: Wilt u een domein of e-mailafzender veilig markeren?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281143"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Wilt u een domein of e-mailafzender veilig markeren?

- Het gebruik van lijsten met **veilige afzenders wordt niet aanbevolen** omdat het uw organisatie openstelt voor spam-, phish- en spoofing-aanvallen.
- Als er echter een zakelijke vereiste is, raden we **u aan** **[hiervoor e-mailstroomregels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken. Onze richtlijnen zorgen ervoor dat afzenderverificatie (controleert of het verzenden van domein niet wordt vervalst). **Opmerking:** We raden u aan valse positieven te beheren door veilige afzenderlijsten te gebruiken, omdat uitzonderingen op spamfiltering uw organisatie kunnen openen voor beveiligingsaanvallen. Als uw gebruiker(s) berichten ontvangt die onjuist zijn gemarkeerd als spam of ongewenste e-mail, u **[berichten en bestanden rapporteren aan Microsoft.](https://protection.office.com/reportsubmission)**
- Veilige afzenders in Outlook, Toegestane afzenderlijst of toegestane domeinlijst in antispambeleid **moeten worden vermeden** omdat afzenders alle spam-, spoof- en phish-beveiliging en afzenderverificatie (SPF, DKIM, DMARC) omzeilen. Deze methode wordt het best alleen gebruikt voor tijdelijke tests.
