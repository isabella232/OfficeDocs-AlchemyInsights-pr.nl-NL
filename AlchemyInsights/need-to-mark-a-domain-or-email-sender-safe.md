---
title: Wilt u een domein of e-mail afzender als veilig markeren?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803240"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Wilt u een domein of e-mail afzender als veilig markeren?

- Het gebruik van **lijsten met veilige afzenders wordt niet aanbevolen** , omdat het uw organisatie opent tegen spam, phishing en spoofing.
- Als er echter wel een zakelijke behoefte is, is het **raadzaam** om hiervoor een **[e-mail stroom regels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken. Onze richtlijnen zorgen voor verificatie van de afzender (verifiëren of verzenden van een domein geen Spoofing wordt). **Opmerking**: het wordt afgeraden dat u onware positieven beheert met behulp van lijsten met veilige afzenders, omdat uitzonderingen op spam filteren uw organisatie kan openen tegen beveiligingsaanvallen. Meld **[berichten en bestanden naar Microsoft](https://protection.office.com/reportsubmission)** als uw gebruikers (en) berichten die niet correct zijn gemarkeerd als spam of ongewenste e-mail, willen ontvangen.
- Veilige afzenders in Outlook, lijst met toegestane afzenders of de lijst met toegestane domeinen in het antispambeleid **moet worden vermeden** omdat afzenders alle spam, spoofing en phishing-bescherming (SPF, dkim, DMARC). Deze methode is het meest geschikt voor tijdelijke tests.
