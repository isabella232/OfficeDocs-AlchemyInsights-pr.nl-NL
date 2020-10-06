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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366423"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Voorwaardelijke toegang voor Exchange controleren

Gebruikers met voorwaardelijke toegang ontvangen een e-mail melding als ze niet voldoen aan de toegangsvereisten van uw organisatie. We raden een of meer van de volgende oplossingen aan om dit op te lossen:

- Als u ervan wordt uitgegaan dat het apparaat is ingeschreven, adviseert u de gebruiker om naar de bedrijfsportal-app te gaan en controleert u of deze wordt weergegeven in de bedrijfsportal. Als dit niet het geval is, moet de gebruiker het apparaat registreren.
- Ga in de Azure-Portal naar intune > apparaatcompatibiliteit. Klik onder monitor op apparaatcompatibiliteit. Bekijk het nalevings rapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.
- Ga in de Azure-Portal naar intune > apparaatcompatibiliteit. Klik onder beheren op beleidsregels. Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruikers. Als u geen profiel hebt toegewezen, kan intune de nalevingsstatus van het apparaat niet bevestigen.
- De voorwaardelijke toegang-opdracht van de gebruiker bewerken.

1. Ga in de Azure-Portal naar **intune**-  >  beleid voor**voorwaardelijke toegang**  >  **Policies**.
2. Selecteer een beleid in de lijst.
3. Klik op gebruikers en groepen.
4. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de lijst toevoegen. Voeg ze toe aan de lijst uitsluiten om ervoor te zorgen dat iemand van het beleid weglaat.

Handige koppelingen:

[Overzicht van apparaatcompatibiliteit](https://docs.microsoft.com/intune/device-compliance-get-started)

[Oplossing van een certificeringsinstantie](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Beleid voor probleemoplossing](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Naleving van intune-apparaat controleren](https://docs.microsoft.com/intune/compliance-policy-monitor)

Opmerking: deze stappen zijn alleen bedoeld voor het oplossen van de voorwaardelijke toegang van de Azure Active Directory-functie. Het is ook mogelijk om een apparaat te gebruiken dat het e-mailadres van de e-mail met Exchange-beleid blokkeert. [Hier](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)vindt u meer informatie over Exchange Device Management.
