---
title: Voorwaardelijke toegang voor Intune bewaken
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427424"
---
# <a name="monitor-intune-conditional-access"></a>Voorwaardelijke toegang voor Intune bewaken

Gebruikers aan wie voorwaardelijke toegang is gericht, ontvangen een e-mailmelding als ze niet aan de toegangsvereisten van uw organisatie voldoen. U wordt aangeraden een of meer van de volgende oplossingen op te lossen:

1. Als ervan wordt uitgegaan dat het apparaat is geregistreerd, adviseert u de gebruiker naar de bedrijfsportal-app te gaan en te controleren of deze wordt weergegeven in de bedrijfsportal. Als dat niet zo is, moet de gebruiker het apparaat registreren.
1. Ga in de Azure Portal naar **Intune**  >  **Device compliance.** 
1. Als u het rapport apparaat compliance wilt bekijken om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel, klikt u onder **Beeldscherm** op **Apparaat compliance.**
1. Ga in de Azure Portal naar **Intune**  >  **Device compliance.** Klik **onder Beheren op** **Beleid.** Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van de gebruiker. Als er geen profiel is toegewezen, kan Intune de compatibiliteitsstatus van het apparaat niet bevestigen.
1. Bewerk de toewijzing van voorwaardelijke toegang van de gebruiker.
1. Navigeer in de Azure Portal naar **Intune-beleidsregels** voor voorwaardelijke toegang, selecteer een beleid in de lijst en klik  >    >  op Gebruikers **en groepen.**
1. Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de **lijst Opnemen.** Als u ervoor wilt zorgen dat een persoon in het beleid wordt **weggelaten,** voegt u deze toe aan de lijst Uitsluiten.

**Handige koppelingen:**

- [Overzicht van apparaat compliance](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Beleid voor probleemoplossing](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune-apparaat compliance bewaken](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Deze stappen zijn alleen nuttig bij het oplossen van problemen met de voorwaardelijke toegang van de Azure Active Directory-functie. Het is ook mogelijk om een apparaat in quarantaine te plaatsen dat e-mailtoegang blokkeert met Exchange-beleid. Meer informatie over Exchange-apparaatbeheer vindt u [**hier.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
