---
title: Voorbeeld van anti-phishingbeleid van Microsoft Defender voor Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744895"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Voorbeeld van anti-phishingbeleid van Microsoft Defender voor Office 365

Met deze instellingen kunt u een beleid met de naam *Domein en CEO inschakelen.* Dit beleid biedt zowel gebruikers- als domeinbescherming tegen imitatie en past vervolgens het beleid toe op alle e-mail die gebruikers binnen het domein ontvangen. Voeg eerst de volgende gegevens toe om het beleid te maken:

- **Naam:** Beschrijving van domein **en** CEO: zorgt ervoor dat de CEO en uw domein niet worden nagebootsd.
  **Toegepast op**: Selecteer **Het domein van de geadresseerde is**. Selecteer **onder Een van deze** opties De optie **Kiezen** en selecteer vervolgens een domein. Selecteer **+ Toevoegen.** Schakel het selectievakje in naast de naam van het domein in de lijst (bijvoorbeeld *contoso.com)* en selecteer **toevoegen.** Selecteer **Gereed**.
- Nadat het beleid is gemaakt, kunt u het beleid verder afstemmen met de volgende opties:
  - **Gebruikers toevoegen om ze te beveiligen:** Voeg in dit voorbeeld minimaal het e-mailadres van de CEO toe.
  - **Domeinen toevoegen om te beveiligen:** Voeg het organisatiedomein toe dat het kantoor van de CEO omvat.
  - **Acties kiezen:** **Als** e-mail wordt verzonden door een nagebootste gebruiker, selecteert u Bericht omleiden naar een ander e-mailadres **en** voert u vervolgens het e-mailadres van de beveiligingsbeheerder *in (bijvoorbeeld securityadmin@contoso.com).* Als **e-mail wordt verzonden door een nagebootsd domein,** selecteert u **Het bericht in quarantaine plaatsen.**
  - **Postvakinformatie:** Deze optie is standaard geselecteerd wanneer u een nieuw anti-phishingbeleid maakt. Laat deze instelling **aan voor** de beste resultaten.
  - **Vertrouwde afzenders en domeinen toevoegen:** Definieer in dit voorbeeld geen overschrijvingen.
- Nadat u de instellingen hebt gecontroleerd, **selecteert** u Dit beleid maken of **Opslaan,** naar eigen goed.

Zie [Anti-phishingbeleid in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235)voor meer informatie.
