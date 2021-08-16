---
title: Intune Voorwaardelijke toegang controleren
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025497"
---
# <a name="monitor-intune-conditional-access"></a>Intune Voorwaardelijke toegang controleren

Gebruikers met voorwaardelijke toegang ontvangen een meldingsbericht als ze niet voldoen aan de toegangsvereisten van uw organisatie. Om dit op te lossen, raden we een of meer van de volgende oplossingen aan:

1. Als wordt vermoed dat het apparaat is geregistreerd, adviseert u de gebruiker om naar de Bedrijfsportal-app te gaan en te controleren of het wordt weergegeven in de Bedrijfsportal. Als dit niet het beste is, moet de gebruiker het apparaat registreren.
1. Ga in de Azure-portal naar **Intune**  >  **Device Compliance.** 
1. Als u het compliancerapport van uw apparaat wilt bekijken om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel, klikt u onder Controleren **op** **Apparaat compliance.**
1. Ga in de Azure-portal naar **Intune**  >  **Device Compliance.** Klik **onder Beheren** op **Beleid.** Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van uw gebruiker. Als er geen profiel is toegewezen, kan Intune de nalevingsstatus van het apparaat niet bevestigen.
1. De toewijzing voor voorwaardelijke toegang van de gebruiker bewerken.
1. Navigeer in de Azure-portal naar Beleid voor voorwaardelijke toegang **in Intune,** selecteer een beleid in de  >    >  lijst en klik op **Gebruikers en groepen.**
1. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de **lijst Opnemen.** Als u ervoor wilt zorgen dat een persoon wordt weggelaten uit het beleid, voegt u deze toe aan de **lijst Uitsluiten.**

**Nuttige koppelingen:**

- [Overzicht van apparaat compliance](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Beleid voor probleemoplossing](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune-apparaat compliance controleren](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Deze stappen zijn alleen handig bij het oplossen van problemen met Azure Active Directory functie Voorwaardelijke toegang. Het is ook mogelijk om een apparaat dat de e-mailtoegang blokkeert in quarantaine te plaatsen met Exchange beleid. Meer informatie over Exchange apparaatbeheer vindt u [**hier.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
