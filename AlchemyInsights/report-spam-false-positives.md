---
title: Wilt u een spam false positive melden bij Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396610"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Hebt u legitieme berichten die worden gemarkeerd als ongewenste e-mail?

Het is frustrerend als een legitiem e-mailbericht in de map Ongewenste e-mail of in Quarantaine wordt geplaatst. Houd rekening met deze meest voorkomende redenen voor fout-positieven:

**Tenant overschrijven (meest voorkomende)** Dit is volledig binnen uw besturingselement om te corrigeren.

Verzend het bericht op Microsoft 365 Defender voor een analyse van het beleid en de regels die van invloed zijn; rescan details zijn binnen enkele minuten beschikbaar.
Controleer of wijzig het beleid of de regels, indien van toepassing. 

**End-User overrides (common)** Dit is volledig binnen uw besturingselement om te corrigeren. 

Verzend het bericht op Microsoft 365 Defender voor een analyse van het beleid en de regels die van invloed zijn; rescan details zijn binnen enkele minuten beschikbaar. 

Als een bericht is geblokkeerd omdat het is verzonden vanaf een adres in de lijst Geblokkeerde afzenders van een gebruiker, bevat de koptekst de Uitspraak spamfilter 'SFV:BLK'.

**E-mailverificatie van afzenders** Dit is gedeeltelijk binnen uw besturingselement om te corrigeren.

Verzend het bericht om fouten in de e-mailverificatie van de afzender op het moment van de bezorging te analyseren. resultaten binnen een dag beschikbaar zijn. 

Als u de eigenaar bent van de verzendende infrastructuur, controleert u hoe u deze uitlijnt met SPF, DKIM en DMARC om ervoor te zorgen dat e-mailsystemen van bestemming berichten vertrouwen die vanuit uw domein zijn verzonden. U kunt ook contact opnemen met de afzenders om hun DNS-configuraties aan te pakken.

**Microsoft filtert vonnissen** Dit is gedeeltelijk binnen uw besturingselement om te corrigeren.

Verzend het bericht en rapporteer het bericht als veilig. rescan resultaten zijn binnen een dag beschikbaar. Gebruik de lijst Tenant toestaan/blokkeren wanneer u het niet eens bent met het filteren van vonnissen in bepaalde situaties. U moet echter niet definitief de filters van Microsoft omzeilen. 

Zie voor meer informatie:

- Schakel uw eindgebruikers in om berichten bij Microsoft in te dienen. Microsoft gebruikt deze inzendingen om de effectiviteit van e-mailbeveiligingstechnologieën te verbeteren en deze worden weergegeven in indieningsrapporten die u kunt gebruiken als indicatie voor het bijwerken van beleid. 

- Zie Berichten verzenden voor analyse als u een korte video wilt bekijken over het indienen van berichten voor [analyse.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Beheerdersinzending gebruiken om verdachte spam, phish, URL's en bestanden naar Microsoft te verzenden](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Lijst met toegestane/geblokkeerde tenants beheren](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Berichtkoppen tegen ongewenste e-mail in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Beveiliging tegen uitgaande spam in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)