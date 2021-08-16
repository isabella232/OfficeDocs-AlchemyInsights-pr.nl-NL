---
title: Voorbeeld van Microsoft Defender voor Office 365 anti-phishingbeleid
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035001"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Voorbeeld van Microsoft Defender voor Office 365 anti-phishingbeleid

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

Zie [Anti-phishingbeleid in](https://go.microsoft.com/fwlink/?linkid=2092235)Microsoft 365.
