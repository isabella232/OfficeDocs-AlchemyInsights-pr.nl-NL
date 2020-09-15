---
title: IP-adres en de client identificeren in controlelogboeken
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668305"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-adres en de client identificeren in controlelogboeken

Het IP-adres dat overeenkomt met een activiteit door een Microsoft 365-gebruiker of-beheerder, wordt weergegeven in de controlelogboeken. De clientinformatie wordt ook vastgelegd. Dit zijn de stappen voor het identificeren van deze informatie:

1. Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/).

2. Ga **naar de pagina zoeken in**het  >  **audit logboek** .

   Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in de lijst **activiteiten** . Als dat niet zo is, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).

   **Opmerking**: in het **activiteiten** menu zijn bepaalde activiteiten mogelijk niet beschikbaar. deze controle items worden echter als resultaat gegeven als de optie **resultaten voor alle activiteiten weergeven** is geselecteerd (standaardinstelling).

3. Geef in het veld **gebruikers** de gebruikersnaam op, selecteer het juiste datumbereik voor de activiteit en klik vervolgens op **zoeken**.

In de resultaten ziet u het IP-adres van de activiteit in het deelvenster resultaten. Selecteer de controlerecord om gedetailleerde informatie weer te geven in het vervolgmenu **Details** (bijvoorbeeld klant, gebruiker die actie heeft uitgevoerd, enzovoort).

Zie voor meer informatie [het IP-adres van de computer die wordt gebruikt om toegang te krijgen tot een gemanipuleerd account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
