---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759214"
---
# <a name="attack-simulator-in-microsoft-365"></a>Aanvals Simulator in Microsoft 365

- Mist u aanvals Simulator? Voor een aanvals Simulator is **Office 365 Advanced Threat Protection (abonnement 2)** of **Office 365 Enterprise E5**vereist. Attack Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection (ATP plan 1), Office 365 Enterprise E3 of een microsoft 365-app voor bedrijven-abonnementen.

- Het account dat u gebruikt om gesimuleerde aanvallen te starten, vereist een globale beheerder of beveiligingsmachtigingen voor de beheerder en meervoudige verificatie (MFA). Zie [het volgende onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor meer informatie over de vereisten voor een aanvals Simulator.

- Belangrijke dingen die u moet weten over zwakke beveiligings simulaties van **Grove wachtwoorden** :

  - Als voor het doelaccount MFA is ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gemanipuleerd (de tweede verificatie factor is niet volledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Eén wachtwoord per regel gebruiken en een lege regel (regeleinde) toevoegen na het laatste wachtwoord in de lijst.

- Belangrijke dingen die u moet weten over simulaties van de verbinding van **spear phishing** :

  - U kunt geen aangepaste waarde voor de URL van de **phishingwebsite aannaam**geven

  - Als een geadresseerde de [invoegtoepassing voor het melden van berichten](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te rapporteren, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: nadat de gesimuleerde aanval is voltooid, kunt u op **Details aanval** klikken om het rapport te bekijken.

- Zie [aanvals Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor uitgebreide instructies en nieuwe functies in aanvals Simulator.
