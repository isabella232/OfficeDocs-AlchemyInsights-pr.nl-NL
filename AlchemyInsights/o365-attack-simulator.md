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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325066"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Ontbreekt Attack Simulator? Voor Attack Simulator **is Microsoft Defender vereist Office 365 plan 2** of Office 365 Enterprise **E5.** Attack Simulator is **niet** opgenomen in Microsoft Defender voor Office 365 Abonnement 1, Office 365 Enterprise E3 of Microsoft 365-apps voor bedrijven abonnementen.

- Voor het account dat u gebruikt om gesimuleerde aanvallen te starten, zijn machtigingen van globale beheerders of beveiligingsbeheerders en meervoudige verificatie (MFA) vereist. Zie dit [onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor meer informatie over de vereisten voor Attack Simulator.

- Belangrijke dingen die u moet weten over brute force-aanvalssimulaties: 

  - Als het doelaccount MFA heeft ingeschakeld en het wachtwoord correct is geraden, wordt het account niet als gecompromitteerd (de tweede verificatiefactor is onvolledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Gebruik één wachtwoord per regel en voeg na het laatste wachtwoord in de lijst een lege regel (retour van het vervoer) toe.

- Belangrijke dingen die u moet weten over De phishing-nasimulaties van **de speer:**

  - U kunt geen aangepaste waarde opgeven voor de URL van de **phishing-aanmeldingsserver.**

  - Als een geadresseerde de invoegvoeging Rapportbericht [inschakelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te melden, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: Nadat de gesimuleerde aanval is voltooid, kunt u op **Details van** aanvallen klikken om het rapport te bekijken.

- Zie Attack Simulator in Microsoft 365 voor gedetailleerde instructies en [nieuwe functies in Attack Simulator.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
