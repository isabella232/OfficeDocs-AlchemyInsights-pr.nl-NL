---
title: Voorbeeld van microsoft Defender voor Office 365-anti-phishingbeleid
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693242"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Voorbeeld van microsoft Defender voor Office 365-anti-phishingbeleid

Met deze instellingen wordt het beleid *Domein en CEO ingeschakeld.* Dit beleid biedt zowel gebruikers- als domeinbeveiliging tegen imitatie en past vervolgens het beleid toe op alle e-mail die wordt ontvangen door gebruikers in het domein. Voeg eerst de volgende informatie toe om het beleid te maken:

- **Naam:** Domein en CEO **Description:** zorgt ervoor dat de CEO en uw domein niet worden gemitmiteerd.
  **Toegepast op:** Selecteer **het domein van de ontvanger.** Selecteer **Onder Een van deze** opties de optie **Kiezen** en selecteer vervolgens een domein. Selecteer **+ Toevoegen.** Schakel het selectievakje in naast de naam van het domein in de lijst (bijvoorbeeld *contoso.com)* en selecteer vervolgens **Toevoegen.** Selecteer **Gereed**.
- Nadat het beleid is gemaakt, kunt u het beleid verder afstemmen met behulp van de volgende opties:
  - **Gebruikers toevoegen om te beschermen:** Voeg voor dit voorbeeld minimaal het e-mailadres van de ceo toe.
  - **Domeinen toevoegen om te beschermen:** voeg het organisatiedomein toe dat het kantoor van de CEO bevat.
  - **Kies acties:** **Als** e-mail wordt verzonden door een gemitmiteerde gebruiker, selecteert u Bericht omleiden naar een ander e-mailadres en voert u het e-mailadres van de beveiligingsbeheerder in (bijvoorbeeld *securityadmin@contoso.com).* Als **e-mail wordt verzonden door een gemitmiteerd domein,** selecteert u **Het bericht in quarantaine plaatsen.**
  - **Postvakinformatie:** deze optie wordt standaard geselecteerd wanneer u een nieuw anti-phishingbeleid maakt. Laat deze instelling **aan voor** de beste resultaten.
  - **Vertrouwde afzenders en domeinen toevoegen:** Definieer in dit voorbeeld geen overschrijvingen.
- Nadat u de instellingen hebt gecontroleerd, selecteert u **Dit beleid maken** of **Opslaan,** waar van toepassing.

Zie [Anti-phishingbeleid in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235)voor meer informatie.
