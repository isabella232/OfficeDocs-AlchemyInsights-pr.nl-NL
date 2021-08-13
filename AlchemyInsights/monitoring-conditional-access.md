---
title: Voorwaardelijke toegang controleren
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975096"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Voorwaardelijke toegang controleren voor Exchange

Gebruikers met voorwaardelijke toegang ontvangen een meldingsbericht als ze niet voldoen aan de toegangsvereisten van uw organisatie. Om dit op te lossen, raden we een of meer van de volgende oplossingen aan:

- Als wordt vermoed dat het apparaat is geregistreerd, adviseert u de gebruiker om naar de Bedrijfsportal-app te gaan en te controleren of het wordt weergegeven in de Bedrijfsportal. Als dit niet het beste is, moet de gebruiker het apparaat registreren.
- Ga in de Azure-portal naar Intune > Apparaat compliance. Klik onder Controleren op Apparaat compliance. Bekijk het rapport apparaat compliance om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.
- Ga in de Azure-portal naar Intune > Apparaat compliance. Klik onder Beheren op Beleid. Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van uw gebruiker. Als er geen profiel is toegewezen, kan Intune de nalevingsstatus van het apparaat niet bevestigen.
- De toewijzing voor voorwaardelijke toegang van de gebruiker bewerken.

1. Ga in de Azure-portal naar **Beleid voor voorwaardelijke toegang in Intune**  >    >  .
2. Selecteer een beleid in de lijst.
3. Klik op Gebruikers en groepen.
4. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de lijst Opnemen. Als u ervoor wilt zorgen dat een persoon wordt weggelaten uit het beleid, voegt u deze toe aan de lijst Uitsluiten.

Nuttige koppelingen:

[Overzicht van apparaat compliance](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Beleid voor probleemoplossing](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune-apparaat compliance controleren](https://docs.microsoft.com/intune/compliance-policy-monitor)

Opmerking: deze stappen zijn alleen handig bij het oplossen van problemen met Azure Active Directory functie Voorwaardelijke toegang. Het is ook mogelijk om een apparaat dat de e-mailtoegang blokkeert in quarantaine te plaatsen met Exchange beleid. Meer informatie over Exchange apparaatbeheer vindt u [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
