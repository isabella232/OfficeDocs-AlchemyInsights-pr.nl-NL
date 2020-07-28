---
title: Apple MDM Push Certificate is niet ingesteld
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439014"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Certificate is niet ingesteld

Een Apple MDM Push Certificate (ook wel bekend als een Apple Push Notification Service (APNS) certificaat) is niet geconfigureerd voor uw abonnement. Zonder een Apple MDM Push Certificate geconfigureerd, u iOS- en Mac OS-apparaten niet inschrijven en beheren. Nadat u het certificaat aan Intune hebt toegevoegd, kunnen gebruikers de Bedrijfsportal-app installeren om hun iOS-apparaten in te schrijven.

1. Selecteer **'Ik ga akkoord'.** om Microsoft toestemming te geven om gegevens naar Apple te verzenden.

2. Selecteer **Uw csr downloaden** van het intune-certificaatondertekeningsverzoek dat nodig is om een Apple MDM-pushcertificaat te maken. Het bestand wordt gebruikt om een vertrouwensrelatiecertificaat aan te vragen bij de Apple Push Certificates Portal.

3. Selecteer **Uw MDM-pushcertificaat maken** om naar de Apple Push Certificates Portal te gaan. Meld u aan bij uw bedrijf Apple ID en selecteer **Vervolgens Een certificaat maken**. Selecteer **Bestand kiezen,** blader naar het aanvraagbestand voor certificaatondertekenen en kies **Upload**. Kies op de pagina Bevestiging **download** om het certificaatbestand (.pem) te downloaden en sla het bestand lokaal op.
 
**Opmerking**: Het certificaat is gekoppeld aan de Apple ID die wordt gebruikt om het te maken. Gebruik als aanbevolen praktijk een Apple ID voor beheertaken en zorg ervoor dat het postvak door meer dan één persoon wordt gecontroleerd of door een distributielijst te gebruiken. Gebruik nooit een persoonlijke Apple ID. Gebruik dezelfde Apple ID om het Apple Push-certificaat elke 12 maanden te verlengen.
 
4. Voer de Apple ID in die wordt gebruikt om uw Apple MDM-pushcertificaat te maken. Neem deze id op als een herinnering voor wanneer u het certificaat moet verlengen.

5. Ga naar het certificaatbestand (.pem), kies **Openen**en kies **vervolgens Uploaden**. Met het pushcertificaat kan Intune Apple-apparaten inschrijven en beheren.