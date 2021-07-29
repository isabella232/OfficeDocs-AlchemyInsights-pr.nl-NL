---
title: IP-adres en client identificeren in auditlogboeken
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
ms.openlocfilehash: a596dd4bed90a0d777dcf19c4c82b41c67fac812
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630280"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-adres en client identificeren in auditlogboeken

Het IP-adres dat overeenkomt met een activiteit van een Microsoft 365 gebruiker of beheerder wordt weergegeven in de auditlogboeken. De clientgegevens worden ook vastgelegd. Hier volgen de stappen voor het identificeren van dergelijke informatie

1. Meld u aan bij [Microsoft 365 compliancecentrum.](https://protection.office.com/)

2. Ga naar de **zoekpagina**  >  **Van het zoeklogboek zoeken.**

   Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in **de lijst** Activiteiten. Als dit niet het beste is, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).

   **Opmerking:** Bepaalde activiteiten zijn mogelijk niet beschikbaar in **het** menu Activiteiten; Deze audititems worden echter geretourneerd als **Resultaten voor** alle activiteiten tonen is geselecteerd (standaardinstelling).

3. Geef de gebruikersnaam op in **het veld Gebruikers,** selecteer het juiste datumbereik voor de activiteit en klik vervolgens op **Zoeken**.

In de resultaten ziet u het IP-adres voor die activiteit in het resultatenvenster. Selecteer de auditrecord voor gedetailleerde informatie in de flyout **Details** (bijvoorbeeld Client, Gebruiker die actie heeft uitgevoerd, enzovoort).

Zie Het IP-adres zoeken van de computer die wordt gebruikt voor toegang tot [een gekromd account](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)voor meer informatie.
