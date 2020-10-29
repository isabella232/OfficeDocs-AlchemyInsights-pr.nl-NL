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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801546"
---
# <a name="attack-simulator-in-microsoft-365"></a>Aanvals Simulator in Microsoft 365

- Mist u aanvals Simulator? Voor de aanvals Simulator is **Microsoft Defender for Office 365 plan 2 (ATP abonnement 2)** of **Office 365 Enterprise E5** vereist. Er is **geen** aanvals Simulator opgenomen in Microsoft Defender for Office 365 plan 1 (ATP plan 1), Office 365 Enterprise E3 of microsoft 365-apps voor Business-abonnementen.

- Het account dat u gebruikt om gesimuleerde aanvallen te starten, vereist een globale beheerder of beveiligingsmachtigingen voor de beheerder en meervoudige verificatie (MFA). Zie [het volgende onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor meer informatie over de vereisten voor een aanvals Simulator.

- Belangrijke dingen die u moet weten over zwakke beveiligings simulaties van **Grove wachtwoorden** :

  - Als voor het doelaccount MFA is ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gemanipuleerd (de tweede verificatie factor is niet volledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Eén wachtwoord per regel gebruiken en een lege regel (regeleinde) toevoegen na het laatste wachtwoord in de lijst.

- Belangrijke dingen die u moet weten over simulaties van de verbinding van **spear phishing** :

  - U kunt geen aangepaste waarde voor de URL van de **phishingwebsite aannaam** geven

  - Als een geadresseerde de [invoegtoepassing voor het melden van berichten](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te rapporteren, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: nadat de gesimuleerde aanval is voltooid, kunt u op **Details aanval** klikken om het rapport te bekijken.

- Zie [aanvals Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor uitgebreide instructies en nieuwe functies in aanvals Simulator.
