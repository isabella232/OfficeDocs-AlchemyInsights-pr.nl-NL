---
title: 2681 aanvals Simulator in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305327"
---
# <a name="attack-simulator-in-office-365"></a>Aanvals Simulator in Office 365

- Mist u Attack Simulator? Voor aanvals Simulator is **office 365 Advanced Threat Protection Plan 2 (ATP-abonnement 2)** of **Office 365 Enterprise E5**vereist. Aanvals Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection Plan 1 (ATP-abonnement 1), Office 365 Enterprise E3 of Office 365 Business-abonnementen.

- Het account dat u gebruikt voor het starten van gesimuleerde aanvallen vereist globale beheerder of beveiligingsbeheerder machtigingen en multi-factor Authentication (MFA). Zie [dit onderwerp](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)voor meer informatie over de vereisten van de aanvals Simulator.

- Belangrijke dingen om te weten over **Brute Force Password** Attack simulaties:

  - Als de doelaccount MFA is ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gecompromitteerd (de tweede verificatiefactor is onvolledig).

  - Het wachtwoordbestand mag niet groter zijn dan 10 MB. Gebruik één wachtwoord per regel en neem een lege regel (Return) op na het laatste wachtwoord in de lijst.

- Belangrijke dingen om te weten over **spear phishing** attach simulaties:

  - U geen aangepaste waarde opgeven voor de URL van de **aanmeldingsserver van phishing**.

  - Als een geadresseerde de [invoegtoepassingen rapportbericht inschakelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te rapporteren, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).

- Rapporten: nadat de gesimuleerde aanval is voltooid, u op **aanvals Details** klikken om het rapport te bekijken.

- Zie [aanvals Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor gedetailleerde instructies en nieuwe functies in de aanvals Simulator.
