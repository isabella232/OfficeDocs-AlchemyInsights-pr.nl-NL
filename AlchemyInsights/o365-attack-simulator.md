---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506733"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Mis je Attack Simulator? Attack Simulator vereist **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** of **Office 365 Enterprise E5**. Attack Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 of microsoft 365 Apps voor bedrijven abonnementen.

- Het account dat u gebruikt om gesimuleerde aanvallen te starten, vereist globale beheerders- of beveiligingsbeheerdersmachtigingen en multi-factor authenticatie (MFA). Zie [dit onderwerp voor](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)meer informatie over de vereisten van attack simulator.

- Belangrijke dingen om te weten over **Brute Force Password** aanval simulaties:

  - Als het doelaccount MFA heeft ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gecompromitteerd (de tweede verificatiefactor is onvolledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Gebruik één wachtwoord per regel en voeg een lege lijn (retourvervoer) toe na het laatste wachtwoord in de lijst.

- Belangrijke dingen om te weten over **Spear Phishing** hechten simulaties:

  - Door het ontwerp, u geen aangepaste waarde voor **Phishing login server URL**.

  - Als een ontvanger de [invoegtoepassing Rapportbericht inschakelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te melden, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: Nadat de gesimuleerde aanval is voltooid, u op **Aanvalsdetails** klikken om het rapport te bekijken.

- Zie [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor gedetailleerde instructies en nieuwe functies in Attack Simulator.
