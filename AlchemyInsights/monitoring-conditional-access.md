---
title: Voorwaardelijke toegang bewaken
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708669"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Voorwaardelijke toegang voor Exchange bewaken

Gebruikers aan wie voorwaardelijke toegang is gericht, ontvangen een e-mailmelding als ze niet aan de toegangsvereisten van uw organisatie voldoen. U wordt aangeraden een of meer van de volgende oplossingen op te lossen:

- Als ervan wordt uitgegaan dat het apparaat is geregistreerd, adviseert u de gebruiker naar de bedrijfsportal-app te gaan en te controleren of deze wordt weergegeven in de bedrijfsportal. Als dat niet zo is, moet de gebruiker het apparaat registreren.
- Ga in de Azure-portal naar Intune > apparaat compliance. Klik onder Beeldscherm op Apparaat compliance. Bekijk het apparaat compliance-rapport om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.
- Ga in de Azure-portal naar Intune > apparaat compliance. Klik onder Beheren op Beleid. Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van de gebruiker. Als er geen profiel is toegewezen, kan Intune de compatibiliteitsstatus van het apparaat niet bevestigen.
- Bewerk de toewijzing van voorwaardelijke toegang van de gebruiker.

1. Ga in de Azure-portal naar Beleid voor voorwaardelijke toegang **in Intune.**  >    >  
2. Selecteer een beleid in de lijst.
3. Klik op Gebruikers en groepen.
4. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de lijst Opnemen. Als u ervoor wilt zorgen dat een persoon in het beleid wordt weggelaten, voegt u deze toe aan de lijst Uitsluiten.

Handige koppelingen:

[Overzicht van apparaat compliance](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Beleid voor probleemoplossing](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune-apparaat compliance bewaken](https://docs.microsoft.com/intune/compliance-policy-monitor)

Opmerking: deze stappen zijn alleen handig bij het oplossen van problemen met de voorwaardelijke toegang van de Azure Active Directory-functie. Het is ook mogelijk om een apparaat in quarantaine te plaatsen dat e-mailtoegang blokkeert met Exchange-beleid. Meer informatie over Exchange-apparaatbeheer vindt u [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
