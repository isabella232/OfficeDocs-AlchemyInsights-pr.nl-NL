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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713461"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Mis je Attack Simulator? Attack Simulator vereist **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** of **Office 365 Enterprise E5**. Attack Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 of Microsoft 365 Apps voor zakelijke abonnementen.

- Voor het account dat u gebruikt om gesimuleerde aanvallen uit te voeren, zijn algemene machtigingen voor beheerders of beveiligingsbeheerders en multi-factor authenticatie (MFA) vereist. Zie [dit onderwerp](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)voor meer informatie over de vereisten van Attack Simulator.

- Belangrijke dingen die u moet weten over **Brute Force Password** aanval simulaties:

  - Als het doelaccount MFA heeft ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gecompromitteerd (de tweede verificatiefactor is onvolledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Gebruik één wachtwoord per regel en voeg een lege regel (vervoer retour) toe na het laatste wachtwoord in de lijst.

- Belangrijke dingen die u moet weten over **Spear Phishing** voeg simulaties toe:

  - Door het ontwerp u geen aangepaste waarde opgeven voor **de URL van de phishing-inlogserver.**

  - Als een ontvanger de [invoegtoepassing Rapportbericht](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) inschakelen gebruikt om het bericht als phishing te melden, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: Nadat de gesimuleerde aanval is voltooid, u op **Aanvalsdetails** klikken om het rapport te bekijken.

- Zie [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor gedetailleerde instructies en nieuwe functies in Attack Simulator.
